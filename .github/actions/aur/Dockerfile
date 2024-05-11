FROM docker.io/library/archlinux:base-devel

RUN pacman -Syu --needed --noconfirm pacman-contrib namcap git sudo && \
  useradd -m builder && \
  echo 'builder ALL=(ALL) NOPASSWD: ALL' >> /etc/sudoers

WORKDIR /home/builder
USER builder

# Install paru
RUN git clone https://aur.archlinux.org/paru-bin.git
WORKDIR /home/builder/paru-bin
RUN makepkg -si --noconfirm
COPY . .
USER root 
RUN chown -R builder:builder ./entrypoint.sh
USER builder
RUN chmod +x ./entrypoint.sh
RUN ls -la

ENTRYPOINT [ "./entrypoint.sh" ]
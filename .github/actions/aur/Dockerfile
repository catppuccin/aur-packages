FROM docker.io/library/archlinux:base-devel

RUN pacman -Syu --needed --noconfirm pacman-contrib namcap git sudo && \
  useradd -m builder && \
  echo 'builder ALL=(ALL) NOPASSWD: ALL' >> /etc/sudoers

WORKDIR /home/builder
USER builder

# Looks like paru-bin hasn't been updated yet, so clone paru-git for now?
# ref: https://github.com/Morganamilo/paru/issues/1454#issuecomment-3663567951
#
# RUN git clone https://aur.archlinux.org/paru-bin.git
# WORKDIR /home/builder/paru-bin

# Install paru
RUN git clone https://aur.archlinux.org/paru-git.git
WORKDIR /home/builder/paru-git
RUN makepkg -si --noconfirm
COPY entrypoint.sh /entrypoint.sh
USER root 
RUN chmod +x /entrypoint.sh
USER builder

ENTRYPOINT [ "/entrypoint.sh" ]

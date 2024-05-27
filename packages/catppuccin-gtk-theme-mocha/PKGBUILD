# Maintainer: Catppuccin <releases@catppuccin.com>

pkgname=catppuccin-gtk-theme-mocha
pkgver=1.0.2 # renovate: datasource=github-tags depName=catppuccin/gtk
pkgrel=1
pkgdesc='Soothing pastel theme for GTK - Mocha'
arch=('any')
license=('GPL3')
url='https://github.com/catppuccin/gtk'
source=(
	"$pkgname-$pkgver-blue.zip::$url/releases/download/v$pkgver/catppuccin-mocha-blue-standard+default.zip"
	"$pkgname-$pkgver-flamingo.zip::$url/releases/download/v$pkgver/catppuccin-mocha-flamingo-standard+default.zip"
	"$pkgname-$pkgver-green.zip::$url/releases/download/v$pkgver/catppuccin-mocha-green-standard+default.zip"
	"$pkgname-$pkgver-lavender.zip::$url/releases/download/v$pkgver/catppuccin-mocha-lavender-standard+default.zip"
	"$pkgname-$pkgver-maroon.zip::$url/releases/download/v$pkgver/catppuccin-mocha-maroon-standard+default.zip"
	"$pkgname-$pkgver-mauve.zip::$url/releases/download/v$pkgver/catppuccin-mocha-mauve-standard+default.zip"
	"$pkgname-$pkgver-peach.zip::$url/releases/download/v$pkgver/catppuccin-mocha-peach-standard+default.zip"
	"$pkgname-$pkgver-pink.zip::$url/releases/download/v$pkgver/catppuccin-mocha-pink-standard+default.zip"
	"$pkgname-$pkgver-red.zip::$url/releases/download/v$pkgver/catppuccin-mocha-red-standard+default.zip"
	"$pkgname-$pkgver-rosewater.zip::$url/releases/download/v$pkgver/catppuccin-mocha-rosewater-standard+default.zip"
	"$pkgname-$pkgver-sapphire.zip::$url/releases/download/v$pkgver/catppuccin-mocha-sapphire-standard+default.zip"
	"$pkgname-$pkgver-sky.zip::$url/releases/download/v$pkgver/catppuccin-mocha-sky-standard+default.zip"
	"$pkgname-$pkgver-teal.zip::$url/releases/download/v$pkgver/catppuccin-mocha-teal-standard+default.zip"
	"$pkgname-$pkgver-yellow.zip::$url/releases/download/v$pkgver/catppuccin-mocha-yellow-standard+default.zip"
)
sha256sums=('6f1f41058dfb0008b1c714ec0a000ec35acc95af4d88d142209d654af3800e85'
            'e6a4caee454c5270f3929cb0de4a700efe0303d2a80cd5140746297201bf2da5'
            '38af21acb9656b26b12ece7446bc9ed973610fe7aa979598fa31cba1688dea66'
            '9207591e97d36bc517b1912893624fac25015998f27b24cf6af0cf57fd647259'
            '1d354ee2ca0000134663bbf03997914c2f2d67af5e2280cd28526e51f70bbd5b'
            '8d6474b3699444b4589efc33efbceaefbcb893a843bc849d3ad6b8d911e4d345'
            '6d345edd8071da9be1c277657f8b6f97ffb3dac9601cf7bba541dd646da2e02e'
            '2bce492cbf76dea867b6a4515c0d79ddf195b4ae8e5275980e461661cbef7c87'
            '8f76edf91128c7979173aa0b0b457051028f1ba388e8f85b61bc2767dce4c8d0'
            '64c797786161393300502b0b3a6009d7e24f77418c83bf83c79d4076a164dbc4'
            '41d19c3bf2266d9dd026d4ff2b0b12bdaac7e65119da5d22c78101d207f2883c'
            '1aa182d7aa6c45df44947456ca311e0894388f37eab0679023bbdf6db9c2c5d1'
            '6de3ae753ccffa0b524e59f6eb0189e229145ed5bc013725b745e0efa76f2631'
            'fc501e8ae9c0bc792872ecd7ba674703997c2e24f572713c9c4e11b291b871d6')

package() {
	install -d "$pkgdir/usr/share/themes/"
	cp -r -a --no-preserve=ownership \
		catppuccin-mocha-* "$pkgdir/usr/share/themes"
}

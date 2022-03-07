# Maintainer: Luis Pérez <luis.perez@protonmail.com>
pkgname=pumble-desktop-bin
pkgver=1.3.0
pkgrel=1
pkgdesc='Pumble is a free team alternative to Slack and Microsoft Teams. Unlimited users and history - all for free.'
arch=('x86_64')
url="https://pumble.com"
license=('CUSTOM')
groups=('Internet')
depends=('alsa-lib' 'atk' 'at-spi2-atk' 'at-spi2-core' 'cairo' 'dbus' 'desktop-file-utils' 'expat' 'gdk-pixbuf2' 'glib2' 'gtk3' 'hicolor-icon-theme' 'libappindicator-gtk3' 'libcups' 'libdrm' 'libnotify' 'libsecret' 'libx11' 'libxcb' 'libxcomposite' 'libxdamage' 'libxext' 'libxfixes' 'libxkbcommon' 'libxrandr' 'libxshmfence' 'libxss' 'libxtst' 'mesa' 'nspr' 'nss' 'pango' 'util-linux-libs' 'xdg-utils')
options=('!strip' '!emptydirs')
install=${pkgname}.install
source=("https://pumble.com/download/desktop/linux/Pumble-linux-${pkgver}.deb")
sha256sums=('d9704c7a84c4622b428748eee0a62932afd0d8a003be06feaad3c9a95ba09561')

package(){
	# Extract package data
	tar xf data.tar.xz -C "${pkgdir}"

	install -D -m644 "${pkgdir}/opt/Pumble/LICENSES.chromium.html" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
	install -D -m644 "${pkgdir}/opt/Pumble/LICENSE.electron.txt" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE.electron"

}

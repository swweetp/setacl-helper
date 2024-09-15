# Maintainer: swweetp <48543769+swweetp@users.noreply.github.com>
pkgname=setacl-helper
pkgver=0.1
pkgrel=1
epoch=
pkgdesc="Helper to set ACL using udev rules"
arch=('any')
url=""
license=('unknown')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(
	"script"
	"${pkgname}.conf"
	"80-${pkgname}.rules"
)
noextract=()
sha256sums=('8a9e7ea14ec1167ce2588fa7ef6ceee64cd2f10011e01b280d2853fb93c129b2'
            '91352e7fb4a1579902d2d9d0797b78b2b6cbca4bfb1b6844dc63314c893a0f52'
            'b62223ef1e90a5a0cb6a95b11c0f1e74941289f22c51a4228b51e2a9e1481571')
validpgpkeys=()
backup=(
	"etc/${pkgname}.conf"
)
package() {
	install -Dm644 "${srcdir}/${pkgname}.conf" "${pkgdir}/etc/${pkgname}.conf"
	install -Dm644 "${srcdir}/80-${pkgname}.rules" "${pkgdir}/usr/lib/udev/rules.d/80-${pkgname}.rules"
	install -Dm755 "${srcdir}/script" "${pkgdir}/usr/lib/${pkgname}/script"
}

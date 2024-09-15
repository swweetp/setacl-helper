# Maintainer: swweetp <48543769+swweetp@users.noreply.github.com>
pkgname=setacl-helper
pkgver=0.1
pkgrel=1
epoch=
pkgdesc="Helper to set ACL using udev rules"
arch=('any')
url="https://github.com/swweetp/setacl-helper"
license=('MIT')
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
	"LICENSE"
)
noextract=()
sha256sums=('e52e0cafdcb103191ed120a5ecf9256180d75d077cba6cd14f355c6da8cb82e6'
            '91352e7fb4a1579902d2d9d0797b78b2b6cbca4bfb1b6844dc63314c893a0f52'
            'b62223ef1e90a5a0cb6a95b11c0f1e74941289f22c51a4228b51e2a9e1481571'
            '9f00debbb4574fd2b767acd847fcf17c25bfb8d7cde63084801e94047b84e180')
validpgpkeys=()
backup=(
	"etc/${pkgname}.conf"
)
package() {
	install -Dm644 "${srcdir}/${pkgname}.conf" "${pkgdir}/etc/${pkgname}.conf"
	install -Dm644 "${srcdir}/80-${pkgname}.rules" "${pkgdir}/usr/lib/udev/rules.d/80-${pkgname}.rules"
	install -Dm755 "${srcdir}/script" "${pkgdir}/usr/lib/${pkgname}/script"
	install -Dm644 "${srcdir}/LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

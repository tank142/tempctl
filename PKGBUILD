pkgname=tempctl
pkgver=1
pkgrel=1
arch=('any')
license=('GPL3')
depends=('psmisc' 'coreutils')
source=("tempctl" "tempctl.conf" "tempctl.service")
sha256sums=('SKIP' 'SKIP' 'SKIP')
package() {
	install -Dm755 "${srcdir}"/tempctl.conf "${pkgdir}"/etc/tempctl.conf
	install -Dm755 "${srcdir}"/tempctl.service "${pkgdir}"/usr/lib/systemd/system/tempctl.service
	install -d "${pkgdir}"/usr/bin/
	install -m755 "${srcdir}"/tempctl "${pkgdir}"/usr/bin/
}

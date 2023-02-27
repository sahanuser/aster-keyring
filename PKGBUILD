pkgname=aster-keyring
pkgver=20230227
pkgrel=1
pkgdesc="Aster keyring"
arch=('any')
url="https://github.com/sahanuser/Aster-Linux-ISO"
license=('GPL')
install="${pkgname}.install"
source=('Makefile'
        'aster.gpg'
	'aster-revoked'
	'aster-trusted')
validpgpkeys=('77cb3a785ef1d36ad6a3ff6dedb9b8e88153beb7')
pkgver() {
  date +%Y%m%d
}
md5sums=('e32abc16b1d41dfcd6cb77baece98321'
         '026cd135be474cd39e43331c9809ebcb'
         'd41d8cd98f00b204e9800998ecf8427e'
         '61a1548f37bd5e328f484b9bef43abc1')
package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}

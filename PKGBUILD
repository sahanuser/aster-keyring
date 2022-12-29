pkgname=aster-keyring
pkgver=20221229
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
md5sums=('1f1ea458480425f3d66333d0ba4b676b'
         '026cd135be474cd39e43331c9809ebcb'
         'c8f58f2725aa31ce35521991e2ef6c74'
         '61a1548f37bd5e328f484b9bef43abc1')
package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}

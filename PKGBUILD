# Maintainer: Panda <panda@bredos.org>

pkgname=bredos-mirrorlist
filename=bredos-mirrorlist
pkgver=20230712
pkgrel=1
pkgdesc="BredOS mirrorlist"
arch=('any')
url="https://github.com/BredOS/bredos-mirrorlist"
license=('GPL3')
source=(${filename})
install=${pkgname}.install
sha256sums=('b8d57fe6490bc6f9483bd4d308f1069ba6417d6641bdfeb901c7f6ff63279bd2')

pkgver() {
    date +%Y%m%d
}

package() {
  mkdir -p ${pkgdir}/etc/pacman.d
  install -m644 ${srcdir}/${filename} ${pkgdir}/etc/pacman.d/${filename}-new
}


# Maintainer: Brian Knox <taotetek@gmail.com>

pkgname=libestr
pkgver=0.1.2
pkgrel=2
pkgdesc="essentials for string handling (and a bit more)"
url="http://libestr.adiscon.com/"
arch=('i686' 'x86_64')
license=('LGPL2.1')
depends=()
makedepends=()
optdepends=()
options=()
source=("http://libestr.adiscon.com/files/download/libestr-$pkgver.tar.gz")
md5sums=('30ec4054155dc7d7e9b06418181c4f12')
build() {
  cd ${srcdir}/${pkgname}-${pkgver}
  ./configure --prefix=/usr
  make
}
package() {
  cd ${srcdir}/${pkgname}-${pkgver}
  make install DESTDIR=${pkgdir}
}

# Maintainer: lobotomius at gmail dot com

pkgname=byteboozer
pkgver=1.1
pkgrel=1
pkgdesc="c64 data compression software"
arch=('i686' 'x86_64')
url="http://csdb.dk/release/?id=109317"
license=('unknown')
source=('http://csdb.dk/getinternalfile.php/106578/bb.7z')
md5sums=('07355681bd11f0fd7180ced2b50adb50')
build() {
    cd "$srcdir/bb"
    make
}

package() {
    cd "$srcdir/bb"
    mkdir -p "$pkgdir/usr/bin"
    install -m 755 bb "$pkgdir/usr/bin"
}

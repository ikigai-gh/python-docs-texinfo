# Maintainer: Vladislav Slepov <sadmonad@gmail.com>

pkgname='python-docs-texinfo'
pkgver='3.14.6'
pkgrel=1
pkgdesc="Set of Texinfo documentation for Python"
arch=('any')
license=('GPL')
url="https://python.org/doc"
source=("${pkgname}-${pkgver}.tar.bz2::https://www.python.org/ftp/python/doc/${pkgver}/python-${pkgver}-docs-texinfo.tar.bz2")

package() {
    cd "python-${pkgver}-docs-texinfo"
    install -dm 755 "$pkgdir/usr/share/info"
    cp python.info "$pkgdir/usr/share/info"
    install-info --info-dir "$pkgdir/usr/share/info" python.info
}
sha256sums=('1ca6687c236d8c48d05d4aa468ca9075e70ead7586ce191a98511bddeddb8d5b')

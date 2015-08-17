# Maintainer: Florian Léger <florian6 dot leger at laposte dot net>

pkgname=pyrss2gen
pkgver=1.0.0
pkgrel=3
pkgdesc="A Python library for generating RSS 2.0 feeds."
arch=('any')
url='http://www.dalkescientific.com/Python/PyRSS2Gen.html'
license=('BSD')
depends=('python2')
makedepends=('python2-distribute')
source=("http://www.dalkescientific.com/Python/PyRSS2Gen-${pkgver}.tar.gz")
md5sums=('b37ed0c9cfa4438a73dbbb0207f3aff6')

build() {
  cd "$srcdir/PyRSS2Gen-$pkgver"
  install -Dm644 LICENSE ${pkgdir}/usr/share/licenses/${pkgname}/LICENSE
  python2 setup.py install --root="$pkgdir" || return 1
}


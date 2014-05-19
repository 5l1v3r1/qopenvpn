# Maintainer: Michal Krenek (Mikos) <m.krenek@gmail.com>
pkgname=qopenvpn
pkgver=1.1
pkgrel=1
pkgdesc="Simple OpenVPN GUI written in PyQt for systemd based distributions"
arch=('any')
url="https://github.com/xmikos/qopenvpn"
license=('GPL3')
depends=('python2-pyqt')
source=(https://github.com/xmikos/qopenvpn/archive/$pkgver.tar.gz)

build() {
  cd "$srcdir/$pkgname-$pkgver"
  python2 setup.py build
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  python2 setup.py install --root="$pkgdir"
}

# vim:set ts=2 sw=2 et:

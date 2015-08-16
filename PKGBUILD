# Maintainer: Carl George <carl@carlgeorge.us>
# Contributor: Daniel Micay <danielmicay@gmail.com>
# Contributor: Thomas Weißschuh <thomas_weissschuh lavabit com>

# Please see https://github.com/jkbr/httpie/issues/140.
# Until that issue is resolved, the python3 version of httpie in <community> is useless to me.

pkgname="httpie-compat"
pkgver=0.6.0
pkgrel=1
pkgdesc="a command line HTTP client - python2 compatible version"
arch=('any')
url="https://github.com/jkbr/httpie"
license=('BSD')
depends=('python2-requests' 'python2-pygments')
makedepends=('python2-distribute')
provides=('httpie')
conflicts=('httpie' 'python-httpie' 'python2-httpie' 'python-httpie-git' 'python2-httpie-git')
source=("https://pypi.python.org/packages/source/h/httpie/httpie-${pkgver}.tar.gz")
md5sums=('441b750a527ba8dcec08a275cd97eab9')

package() {
  cd "${srcdir}/httpie-${pkgver}"
  python2 setup.py install --root="${pkgdir}" --optimize=1
}

# vim:set ts=2 sw=2 et:

pkgname=python-cdsapi
pkgver=0.4.0
pkgrel=1
pkgdesc="cdsapi"
arch=(any)
license=('APACHE')
depends=('python-tqdm')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/d6/9e/952b99737b2dfc56229306abdd8f353b9114480db29e379ad2a621b12e6b/cdsapi-0.4.0.tar.gz")
sha256sums=('e2fc7c06c18810b2dea38522e4d41470ab91607a155df7de6a6a8bceea90b39d')

build() {
    cd "$srcdir"/cdsapi-$pkgver
    python setup.py build
}

package() {
    cd "$srcdir"/cdsapi-$pkgver
    python setup.py install -O1 --skip-build --root="$pkgdir"
}

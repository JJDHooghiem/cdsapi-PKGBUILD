pkgname=python-cdsapi
pkgver=0.3.1
pkgrel=1
pkgdesc="cdsapi"
arch=(any)
license=('APACHE')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/74/ee/0d0d26dfad17f948bb7ef377972bc67db29870d710d4f5513b13d5614b12/cdsapi-$pkgver.tar.gz")
sha256sums=('3d80f21c7decf923c0a18b42f30a36a16221787412381322485e8a185f7c9404')

build() {
    cd "$srcdir"/cdsapi-$pkgver
    python setup.py build
}

package() {
    cd "$srcdir"/cdsapi-$pkgver
    python setup.py install -O1 --skip-build --root="$pkgdir"
}

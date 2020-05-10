pkgname=python-bitstring
pkgver=3.1.7
pkgrel=1
pkgdesc='make the creation and analysis of binary data as simple and natural as possible'
arch=('any')
url="https://scott-griffiths.github.io/bitstring/"
license=('MIT')
depends=('python')
options=(!emptydirs)
source=("https://github.com/scott-griffiths/bitstring/archive/bitstring-$pkgver.tar.gz")
sha512sums=('57a48cf279f1e0e2ea8e1ce436cd8c256325f6f9e9ad340b8c28c2954712faf8473e5779aeff4d66b4c596dbeb4cb39ea3328d5c22dcb4d8b0ee0a7098023561')

package() {
  cd bitstring-bitstring-$pkgver
  python setup.py install --root="$pkgdir" --optimize=1
  install -D -m644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

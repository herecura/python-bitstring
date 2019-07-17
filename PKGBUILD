pkgname=python-bitstring
pkgver=3.1.6
pkgrel=1
pkgdesc='make the creation and analysis of binary data as simple and natural as possible'
arch=('any')
url="https://scott-griffiths.github.io/bitstring/"
license=('MIT')
depends=('python')
options=(!emptydirs)
source=("https://github.com/scott-griffiths/bitstring/archive/bitstring-$pkgver.tar.gz")
sha512sums=('d78d91f92f60044948199e4fa5ec48c8007268f725e5230d6c8be44a6ced578e61a2c2f8751822f191a909057f38d358a8c944f357a5f9ea98adb6baae3a0da2')

package() {
  cd bitstring-bitstring-$pkgver
  python setup.py install --root="$pkgdir" --optimize=1
  install -D -m644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

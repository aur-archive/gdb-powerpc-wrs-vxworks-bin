#Maintainer: Alex Brinister (alex_brinister@yahoo.com)
pkgname=gdb-powerpc-wrs-vxworks-bin
pkgver=7.5.1
pkgrel=1
pkgdesc="GDB for the VxWorks 6.3 GCC Toolchain"
arch=('x86_64' 'i686')
provides=('gdb-powerpc-wrs-vxworks')
url="http://firstforge.wpi.edu/sf/projects/c--11_toochain"
license=('GPL')
depends=('gdb')
options=('!strip' 'libtool' '!zipman')
if test "$CARCH == x86_64"; then
source=(https://www.dropbox.com/s/fum5axok69zx0q1/$pkgname-$pkgver-$CARCH.tar.xz)
sha512sums=('5b4c5535049a450ab64851b42771fe039da7aab36e61b546404b14cc3242188ba0f55940a362985b2506471d8bfad1f618bb87c585dd8c1b7bdc3b2fd221ead9')
fi

package() {
  cd "$srcdir/$pkgname-$pkgver"
  cp -dpr --no-preserve=ownership ./usr $pkgdir/
}

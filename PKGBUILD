pkgname=wimax_tray
pkgver=0.6
pkgrel=1
pkgdesc="Tray icon for madwimax and Yota written in pygtk"
url="http://zhulik.homelinux.org"
arch=('any')
license=('GPL')
depends=('pygtk' 'python-notify' 'gksu' 'madwimax')
makedepends=()
source=(http://zhulik.homelinux.org/$pkgname-$pkgver.tar.gz)
md5sums=('df04cbb89dcfedd4aea2fb8cd847ac4e')

build() {
  cd $srcdir/$pkgname-$pkgver
  mkdir -p $pkgdir/usr/share/pixmaps
  mkdir -p $pkgdir/usr/bin
  cp -r icons/* $pkgdir/usr/share/pixmaps
  cp wimax_tray.py $pkgdir/usr/bin/$pkgname
  chmod 755 $pkgdir/usr/bin/$pkgname
}


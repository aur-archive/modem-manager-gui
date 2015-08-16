# Maintainer: Ilya Medvedev <medved55rus [at] gmail [dot] com>

pkgname=modem-manager-gui
pkgver=0.0.16
pkgrel=1
pkgdesc="Frontend for ModemManager daemon able to control specific modem functions."
arch=('x86_64' 'i686')
url="http://linuxonly.ru"
license=('GPLv3')
depends=('gtk3>=3.4.0' 'glib2>=2.32.1' 'gdbm>=1.10' 'libnotify>=0.7.5')
makedepends=('pkgconfig')
source=("http://linuxonly.ru/cms/request.php?22")
md5sums=('b474224faa101cf00ff01f5bae2a9964')
 
build() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  ./configure
  make
}
 
package() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  make DESTDIR="${pkgdir}" install
}

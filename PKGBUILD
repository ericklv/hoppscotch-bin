pkgname=hoppscotch-bin
_tag=26.8.2-0
pkgver=${_tag//-/.}
pkgrel=1
pkgdesc="Desktop App for hoppscotch.io"
arch=('x86_64')
url="https://hoppscotch.io"
license=('MIT')
depends=('webkit2gtk-4.1' 'gtk3')
provides=('hoppscotch')
conflicts=('hoppscotch')
options=('!strip' '!debug')
source=("https://github.com/hoppscotch/releases/releases/download/v$_tag/Hoppscotch_linux_x64.deb")
sha256sums=('9a1535253ef4267964fedbcdba4186433e6520065ad4bdac28fd15779ec0c864')

package() {
  bsdtar -xf data.tar.gz -C "$pkgdir"
}

# Maintainer : Igor Duarte Cardoso <igordcard@gmail.com>
# Contributor: jsteel <mail at jsteel dot org>
# Contributor: Renato Coutinho <renato.coutinho@gmail.com>

pkgname=symphonic
_pkgname=${pkgname//s/JS}
pkgver=0.3.0
pkgrel=4
pkgdesc="A portable MP3/WMA/OGG/FLAC file manager for Sony players. Was JSymphonic"
_pkgdesc=Ode_To_Freedom
arch=('any')
url="http://sourceforge.net/projects/symphonic"
depends=('java-environment')
replaces=('jsymphonic')
license=('GPL')
source=(http://downloads.sourceforge.net/project/$pkgname/j${pkgname}/JSymphonic%20version%20${pkgver}%20Ode%20To%20Freedom/JSymphonic_v${pkgver}_$_pkgdesc.zip
        $pkgname)
md5sums=('eccd8934167d2393c7fed3454d5d345c'
         'baf8a1eeabbd1e0b0f35fef5bb788df0')

package() {
  install -Dm644 "$srcdir"/${_pkgname}_v${pkgver}_$_pkgdesc.jar "$pkgdir"/usr/share/$pkgname/$_pkgname.jar
  install -Dm755 "$srcdir"/$pkgname "$pkgdir"/usr/bin/$pkgname
}

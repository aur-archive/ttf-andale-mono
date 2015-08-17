# Maintainer: Viliam Pucik <viliam dot pucik at gmail dot com>
pkgname=ttf-andale-mono
pkgver=1.0
pkgrel=3
pkgdesc="Andale Mono TTF Font from Microsoft"
arch=('any')
url="http://corefonts.sourceforge.net/"
license=('custom:microsoft')
depends=('fontconfig' 'xorg-font-utils')
makedepends=('libarchive>=3.0.2')
#conflicts=('ttf-ms-fonts')
install=$pkgname.install
source=(http://downloads.sourceforge.net/corefonts/andale32.exe LICENSE)
md5sums=('cbdc2fdd7d2ed0832795e86a8b9ee19a'
         'ebe2e15f556ab890d315e32166efe2ae')
sha512sums=('7099c389126d2af146ff082a840c77787f28e59cc8b5fd4147b9a45a34c649bc69ba6ec7c338703950389fce3ac3a7f118f503b7434c7ceb54c89d6210508bd4'
            '100bbc3a1ab97af367b57c137258148d269a78af8afe647d4d4d5db32facb459cb8e66a99078e2ef45d1fe3ca97548f2db0ef589a3a14567145673e03e5f8733')

build() {
  install -dm755 "${pkgdir}/usr/share/fonts/TTF"
  install -m644 AndaleMo.TTF "${pkgdir}/usr/share/fonts/TTF/andalemo.ttf"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}

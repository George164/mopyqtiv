# Скрипт сборки пакета для систем arch linux
# Автор: Евгений

pkgname=mopyqtiv
pkgver=0.1
pkgrel=2
pkgdesc='Mouse oriented PyQt5 image viewer'
arch=('i686' 'x86_64')
url="https://github.com/inaugurator/mopyqtiv"
license=('Apache 2.0')
depends=('python' 'python-pillow' 'python-pyqt5')
provides=('mopyqtiv')
source=("git+https://github.com/inaugurator/mopyqtiv.git")
sha256sums=('SKIP')

package() {

    cd ${pkgname}

    install -m755 -D "${pkgname}" "$pkgdir/usr/bin/mopyqtiv"
    
    gzip -9 "${pkgname}.1"
    install -m644 -D "${pkgname}.1.gz" "$pkgdir/usr/share/man/ru/man1/mopyqtiv.1.gz"
    
    install -m644 -D "${pkgname}.desktop" "$pkgdir/usr/share/applications/mopyqtiv.desktop"
}

# vim: set ts=4 sw=4 tw=0 noet :

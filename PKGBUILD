# Maintainer: Your Name <tmpstpdwn@tuta.io>

pkgname=trashx
pkgver=1.0
pkgrel=1
pkgdesc="A custom trash management system for moving, listing, and restoring files."
arch=('any')
url="https://github.com/tmpstpdwn/trashx"
license=('GPL3')
depends=('bash' 'coreutils' 'util-linux-libs' 'csvlens')
source=('src/trashx')
md5sums=('SKIP')

package() {
    install -Dm755 "$srcdir/trashx" "$pkgdir/usr/bin/trashx"
    install -Dm644 "$srcdir/../LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
    install -Dm644 "$srcdir/../README.md" "$pkgdir/usr/share/doc/$pkgname/README.md"
}

prepare() {
    cp -r "$srcdir/../src" "$srcdir"
}

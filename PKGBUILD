# Maintainer: Eihdran Lego <hadean-eon-dev@proton.me>
pkgname=archinstall-contrib
pkgver=1.0.0
pkgrel=1
pkgdesc="Wrapper scripts for archinstall collaboration and development"
arch=('any')
url="https://github.com/h8d13/archinstall-contrib"
license=('GPL')
depends=('git' 'python')
source=("$pkgname-$pkgver.tar.gz::https://github.com/h8d13/$pkgname/archive/refs/tags/v$pkgver.tar.gz")
sha256sums=('SKIP')

package() {
    cd "$startdir"

    # Install main wrapper
    install -Dm755 ac "$pkgdir/usr/bin/ac"

    # Install all library scripts
    install -dm755 "$pkgdir/usr/lib/ac"
    install -Dm755 aic-lib/* "$pkgdir/usr/lib/ac/"
}

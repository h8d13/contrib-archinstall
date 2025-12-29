# Maintainer: Eihdran Lego <hadean-eon-dev@proton.me>
pkgname=archinstall-contrib
pkgver=1.0.0
pkgrel=1
pkgdesc="Wrapper scripts for archinstall collaboration and development"
arch=('any')
url="https://github.com/h8d13/archinstall-contrib"
license=('GPL')
depends=('git' 'python')
makedepends=('git')
source=("git+https://github.com/h8d13/archinstall-contrib.git")
sha256sums=('SKIP')

package() {
    cd "$srcdir/$pkgname"

    # Install main wrapper
    install -Dm755 ac "$pkgdir/usr/bin/ac"

    # Install all library scripts
    install -dm755 "$pkgdir/usr/lib/ac"
    cp -r aic-lib/* "$pkgdir/usr/lib/ac/"
    chmod -R 755 "$pkgdir/usr/lib/ac"
}

# Maintainer: Eihdran Lego <hadean-eon-dev@proton.me>
pkgname=archinstall-contrib
pkgver=1.0.0
pkgrel=0
pkgdesc="Wrapper scripts for archinstall collaboration and development"
arch=('any')
url="https://github.com/h8d13/archinstall-contrib"
depends=('git' 'python')

package() {
    cd "$startdir"

    # Install main wrapper
    install -Dm755 ac "$pkgdir/usr/bin/ac"

    # Install all library scripts
    install -dm755 "$pkgdir/usr/lib/aic"
    install -Dm755 aic-lib/* "$pkgdir/usr/lib/aic/"
}

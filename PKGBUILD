pkgname=aureus
pkgver=1.0.0
pkgrel=1 
pkgdesc='a minimal AUR helper'
arch=('any')
license=('GPL-3.0-or-later')
depends=('bash' 'pacman' 'fzf' 'git' 'less' 'sed' 'gzip' 'jq')
source=('aureus' 'aureus-jq')
package() {
    install -Dm755 aureus ${pkgdir}/usr/bin/aureus
    install -Dm644 aureus-jq ${pkgdir}/usr/lib/${pkgname}/aureus-jq
}
sha256sums=('d337e74ae4f71a09b488db832867f33ef4725acea3e9b36adc3c8a38251968a1'
            'f7ca43ff8730040a3e59f705241eca05af784244506818681efa052646848e7c')

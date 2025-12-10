pkgname=aureus
pkgver=1.0.1
pkgrel=1
pkgdesc='a minimal AUR helper'
url='https://github.com/wsbankenstein/aureus'
arch=('any')
license=('GPL-3.0-or-later')
depends=('bash' 'pacman' 'fzf' 'git' 'less' 'sed' 'gzip' 'jq')
source=('aureus' 'aureus-jq')
package() {
    install -Dm755 aureus ${pkgdir}/usr/bin/aureus
    install -Dm644 aureus-jq ${pkgdir}/usr/lib/${pkgname}/aureus-jq
}
sha256sums=('55dee08066e0f9860bf2accc35663c123a18d4a301fbaf4dc2931f0a0046987c'
            'fd3b51632457bbc53f433d16605e3c1fd767dba665b4f3d476ef5ad92525b674')

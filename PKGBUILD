pkgname=aureus
pkgver=1.1.0
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
sha256sums=('6ac0141a817222c34324320838bf110d2018fc6920b2bf8d6aa37919334dea7f'
            'fd3b51632457bbc53f433d16605e3c1fd767dba665b4f3d476ef5ad92525b674')

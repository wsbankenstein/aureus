pkgname=aureus
pkgver=1.2.0
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
sha256sums=('ffc96b5b9c461ff3c4bcf722c703b3e0f853872bc9cdad2c2bcbc5297936b8e9'
            'fd3b51632457bbc53f433d16605e3c1fd767dba665b4f3d476ef5ad92525b674')

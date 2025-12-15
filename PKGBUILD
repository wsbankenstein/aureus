pkgname=aureus
pkgver=1.3.1
pkgrel=1
pkgdesc='a minimal AUR helper'
url='https://github.com/wsbankenstein/aureus'
arch=('any')
license=('GPL-3.0-or-later')
depends=('bash' 'pacman' 'fzf' 'git' 'less' 'sed' 'gzip' 'jq' 'awk')
source=('aureus' 'aureus-jq')
package() {
    install -Dm755 aureus ${pkgdir}/usr/bin/aureus
    install -Dm644 aureus-jq ${pkgdir}/usr/lib/${pkgname}/aureus-jq
}
sha256sums=('91ccb3929f37e027a7f4e1d1d5abc0ab42b67d966277122bd1849c5a1ecbf7b4'
            'fd3b51632457bbc53f433d16605e3c1fd767dba665b4f3d476ef5ad92525b674')

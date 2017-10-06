# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=obarun-libs
pkgver=0.1.3
pkgrel=2
pkgdesc="Common functions for obarun program"
arch=(x86_64)
url="https://github.com/Obarun/obarun-libs"
license=('BEERWARE')
depends=('bash' 'git' 'pacman' 'obarun-keyring')
makedepends=('git')
_commit=6826cac675b5fdb3a42c7ae00890a9088d408af2 # tag 0.1.3 fix tags on check_update function at pac.sh files
#source=("obarun-libs::git+https://github.com/Obarun/obarun-libs#tag=v${pkgver}")
source=("obarun-libs::git+https://github.com/Obarun/obarun-libs#commit=${_commit}")
md5sums=('SKIP')
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC') # Eric Vidal

package() {
	cd "${pkgname}"

	make DESTDIR="$pkgdir" install
}


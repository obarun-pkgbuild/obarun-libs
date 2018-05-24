# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=obarun-libs
pkgver=0.1.4
pkgrel=1
pkgdesc="Common functions for obarun program"
arch=(x86_64)
url="https://github.com/Obarun/obarun-libs"
license=('BEERWARE')
depends=('bash' 'git' 'pacman' 'obarun-keyring')
makedepends=('git')
#_commit=a3366f460e037b282cf0ab9cef05ca2d199c0c40 # tag 0.1.3 fix sudo owner without asking for root
source=("obarun-libs::git+https://github.com/Obarun/obarun-libs#tag=v${pkgver}")
#source=("obarun-libs::git+https://github.com/Obarun/obarun-libs#commit=${_commit}")
md5sums=('SKIP')
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC') # Eric Vidal

package() {
	cd "${pkgname}"

	make DESTDIR="$pkgdir" install
}


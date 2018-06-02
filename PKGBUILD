# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=obarun-libs
pkgver=0.1.4
pkgrel=2
pkgdesc="Common functions for obarun program"
arch=(x86_64)
url="https://github.com/Obarun/obarun-libs"
license=('BEERWARE')
depends=('bash' 'git' 'pacman' 'obarun-keyring')
makedepends=('git')
_commit=74cc167a885b27e716c19671a8b210faacd3a2e6 # tag 0.1.4 mount_umount change
#source=("obarun-libs::git+https://github.com/Obarun/obarun-libs#tag=v${pkgver}")
source=("obarun-libs::git+https://github.com/Obarun/obarun-libs#commit=${_commit}")
md5sums=('SKIP')
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC') # Eric Vidal

package() {
	cd "${pkgname}"

	make DESTDIR="$pkgdir" install
}


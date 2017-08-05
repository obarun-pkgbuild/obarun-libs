# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=obarun-libs
pkgver=0.1.2
pkgrel=1
pkgdesc=" Common functions for obarun program"
arch=(x86_64)
url="https://github.com/Obarun/obarun-libs"
license=('BEERWARE')
depends=('bash' 'git' 'pacman' 'obarun-keyring')
makedepends=('git')
backup=()
install=
source=("obarun-libs::git+https://github.com/Obarun/obarun-libs#tag=v${pkgver}")
md5sums=('SKIP')
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC') # Eric Vidal


package() {
	cd "$srcdir/$pkgname"
	install -Dm 0755 "util.sh" "$pkgdir/usr/lib/obarun/util.sh"
	
	install -dm 0755 "$pkgdir/usr/lib/obarun/lib/"
	for file in lib/{custom.sh,filesystem.sh,msg.sh,pac.sh,search.sh};do
		install -Dm 0755 "${file}" "$pkgdir/usr/lib/obarun/lib/"
	done
	
	install -Dm 0644 "LICENSE" "$pkgdir/usr/share/licenses/obarun-libs/LICENSE"
}


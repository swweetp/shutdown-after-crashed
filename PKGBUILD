# Maintainer: Your Name <youremail@domain.com>
pkgname=shutdown-after-crashed
pkgver=1.0
pkgrel=1
epoch=
pkgdesc="systemd service to shutdown the system next time it boots after a crash"
arch=('any')
url=""
license=('MIT')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("$pkgname.service"
        "last-shutdown-unexpected.service"
		"last-shutdown-unexpected.target")
noextract=()
sha256sums=('d798dcd47926f3bf9c841c79deb5c8234b9d70c9a92965268fd520560abe149b'
            '605608334dce306a0e339f359ea505c8f27eb904fe6c8314f957acc3141f8685'
            'f3021f693d08b1dbe1ec013f9767b3300c81c3e13654e4b38a384887d52c60fb')
validpgpkeys=()

package() {
	install -Dm644 "$srcdir/$pkgname.service" "$pkgdir/usr/lib/systemd/system/$pkgname.service"
	install -Dm644 "$srcdir/last-shutdown-unexpected.service" "$pkgdir/usr/lib/systemd/system/last-shutdown-unexpected.service"
	install -Dm644 "$srcdir/last-shutdown-unexpected.target" "$pkgdir/usr/lib/systemd/system/last-shutdown-unexpected.target"
}

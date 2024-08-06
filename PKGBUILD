# Maintainer: swweetp <48543769+swweetp@users.noreply.github.com>
pkgname=shutdown-after-crashed
pkgver=1.0
pkgrel=1
epoch=
pkgdesc="systemd service to shutdown the system next time it boots after a crash"
arch=('any')
url="https://github.com/swweetp/shutdown-after-crashed"
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
		"LICENSE")
noextract=()
sha256sums=('5a9a11032d4b2ee2fc80307ea63efab5d4d297a3d28f68413797a0adf33a95a9'
            '9f00debbb4574fd2b767acd847fcf17c25bfb8d7cde63084801e94047b84e180')
validpgpkeys=()

package() {
	install -Dm644 "$srcdir/$pkgname.service" -t "$pkgdir/usr/lib/systemd/system/"
	install -Dm644 "$srcdir/LICENSE" -t "$pkgdir/usr/share/licenses/$pkgname/"
}

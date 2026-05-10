# Maintainer: Aditya contact@aditya-verma.me
pkgname=fzwall
pkgver=1.0.0
pkgrel=1
pkgdesc="A fuzzel-based wallpaper picker supporting multiple WMs and wallpaper setters"
arch=('any')
url="https://github.com/yourusername/fzwall"
license=('MIT')
depends=('fuzzel')
optdepends=(
    'swaybg: Wayland wallpaper setter (sway)'
    'swww: Wayland wallpaper setter with animations (hyprland)'
    'feh: X11 wallpaper setter'
    'nitrogen: X11 wallpaper setter with GUI'
    'xwallpaper: Lightweight X11 wallpaper setter'
    'libnotify: Desktop notifications support'
)
source=("$pkgname-$pkgver.tar.gz::$url/archive/v$pkgver.tar.gz")
sha256sums=('SKIP') # replace with actual hash: curl -sL <tarball_url> | sha256sum

package() {
    cd "$srcdir/$pkgname-$pkgver"
    install -Dm755 fzwall "$pkgdir/usr/bin/fzwall"
    install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
    install -Dm644 README.md "$pkgdir/usr/share/doc/$pkgname/README.md"
}

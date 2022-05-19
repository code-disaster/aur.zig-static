# Maintainer: Henry Nelson <hcnelson99@gmail.com>
pkgname=zig-static
pkgver=0.10.0
pkgrel=1
zigver=-dev.2306+50a5ddecc
epoch=
pkgdesc="robust, optimal, and clear programming language"
arch=('x86_64' 'aarch64')
url="https://ziglang.org/"
license=('MIT')
depends=()
makedepends=()
options=('!strip')
provides=('zig')
conflicts=('zig')
source_x86_64=("https://ziglang.org/builds/zig-linux-x86_64-$pkgver$zigver.tar.xz")
source_aarch64=("https://ziglang.org/builds/zig-linux-aarch64-$pkgver$zigver.tar.xz")
md5sums_x86_64=('2c960ed07491e228664f6d53687f9d3f')
md5sums_aarch64=('bbe1a9f3db2022fa8a53c0e244824fb1')

package() {
    cd "$srcdir/zig-linux-${CARCH}-$pkgver"
    install -D zig "$pkgdir/usr/bin/zig"
    install -D LICENSE "$pkgdir/usr/share/licenses/zig/LICENSE"
    cp -r lib "$pkgdir/usr"
    install -d "$pkgdir/usr/share/doc"
    cp -r docs "$pkgdir/usr/share/doc/zig"
}

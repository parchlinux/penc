#!/usr/bin/env bash

pkgname=penc
pkgver=1.0.0
pkgrel=1
pkgdesc="parch linux encrypted compress"
arch=("any")
url="https://parchlinux.com/"
license=("GPL")
conflict=("${pkgname%}")
depends=("zstd" "tar" "openssl")
build(){
    cd ${srcdir}
    amber main.ab penc
}
package() {
    cd "$srcdir"
    install -Dm755 penc "$pkgdir/usr/bin/penc"

}


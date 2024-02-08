# Maintainer: Chaiwat Suttipongsakul <cwt@bashell.com>

pkgbase='mkimg-th1520'
pkgname='th1520-firmware'
pkgdesc='TH1520 firmware'
pkgver=20240202
pkgrel=1
url='https://github.com/revyos/mkimg-th1520'
arch=(riscv64)
license=('proprietary')
options=('!strip')
source=("https://github.com/revyos/${pkgbase}/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('65b317ce00ac2d5e2977bfed45b23e1511887a31a72bd569f8d853a68713d96e')

package() {
  cd "$srcdir/$pkgbase-$pkgver/addons/lib/firmware"
  mkdir -p ${pkgdir}/usr/lib/firmware
  cp -a * ${pkgdir}/usr/lib/firmware/
}

# vim:set ts=8 sts=2 sw=2 et:

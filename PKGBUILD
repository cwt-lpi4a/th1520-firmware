# Maintainer: Chaiwat Suttipongsakul <cwt@bashell.com>

pkgbase='mkimg-th1520'
pkgname='th1520-firmware'
pkgdesc='TH1520 firmware'
pkgver=20240720
pkgrel=1
url='https://github.com/revyos/mkimg-th1520'
arch=(riscv64)
license=('proprietary')
options=('!strip')
source=("https://github.com/revyos/${pkgbase}/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('f2983044d141a45f12b842e18d92c7211352479a8e65674de7a61e442f9b02c3')

package() {
  cd "$srcdir/$pkgbase-$pkgver/addons/lib/firmware"
  mkdir -p ${pkgdir}/usr/lib/firmware
  cp -a * ${pkgdir}/usr/lib/firmware/
}

# vim:set ts=8 sts=2 sw=2 et:

# Maintainer: Chaiwat Suttipongsakul <cwt@bashell.com>

pkgbase='mkimg-th1520'
pkgname='th1520-firmware'
pkgdesc='TH1520 firmware'
pkgver=20240127
pkgrel=1
url='https://github.com/revyos/mkimg-th1520'
arch=(riscv64)
license=('proprietary')
options=('!strip')
source=("https://github.com/revyos/${pkgbase}/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('58ea5405fc931f5d091c709e74c5473de1c53588c2b65314ace0a1c35eb1cdb1')

package() {
  cd "$srcdir/$pkgbase-$pkgver/addons/lib/firmware"
  mkdir -p ${pkgdir}/usr/lib/firmware
  cp -a * ${pkgdir}/usr/lib/firmware/
}

# vim:set ts=8 sts=2 sw=2 et:

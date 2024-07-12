# Maintainer: Chaiwat Suttipongsakul <cwt@bashell.com>

pkgbase='mkimg-th1520'
pkgname='th1520-firmware'
pkgdesc='TH1520 firmware'
pkgver=20240602
pkgrel=1
url='https://github.com/revyos/mkimg-th1520'
arch=(riscv64)
license=('proprietary')
options=('!strip')
source=("https://github.com/revyos/${pkgbase}/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('75ea38cc58cd5b1e25f3c93ea9f7111e2b0ac69ef8e5f16419cbd88aa2e94143')

package() {
  cd "$srcdir/$pkgbase-$pkgver/addons/lib/firmware"
  mkdir -p ${pkgdir}/usr/lib/firmware
  cp -a * ${pkgdir}/usr/lib/firmware/
}

# vim:set ts=8 sts=2 sw=2 et:

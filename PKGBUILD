# Maintainer: BuzzStro <https://github.com/BuzzStro/BuzzStro>
pkgname=buzz-scripts
pkgver=1.0
pkgrel=1
pkgdesc="Scripts that display ASCII art "
arch=('any')
license=('MIT')
source=("buzz-arch.sh" "buzz-fedora.sh" "buzz-debian.sh" "buzz.sh" "buzz--h.sh")
md5sums=('SKIP' 'SKIP' 'SKIP' 'SKIP' 'SKIP')  # Gerçek checksum kullanabilirsiniz veya 'SKIP' bırakabilirsiniz

package() {
  # Arch betiğini /usr/bin dizinine kopyala ve izinlerini ayarla
  install -Dm755 "${srcdir}/buzz-arch.sh" "${pkgdir}/usr/bin/buzz-arch"

  # Fedora betiğini /usr/bin dizinine kopyala ve izinlerini ayarla
  install -Dm755 "${srcdir}/buzz-fedora.sh" "${pkgdir}/usr/bin/buzz-fedora"

  # Debian betiğini /usr/bin dizinine kopyala ve izinlerini ayarla
  install -Dm755 "${srcdir}/buzz-debian.sh" "${pkgdir}/usr/bin/buzz-debian"

  # buzz.sh betiğini /usr/bin dizinine kopyala ve izinlerini ayarla
  install -Dm755 "${srcdir}/buzz.sh" "${pkgdir}/usr/bin/buzz"

  # buzz--h.sh betiğini /usr/bin dizinine kopyala ve izinlerini ayarla
  install -Dm755 "${srcdir}/buzz--h.sh" "${pkgdir}/usr/bin/buzz--h"

  # Dosyaların çalıştırma izni olduğundan emin ol
  chmod u+x "${pkgdir}/usr/bin/buzz-arch"
  chmod u+x "${pkgdir}/usr/bin/buzz-fedora"
  chmod u+x "${pkgdir}/usr/bin/buzz-debian"
  chmod u+x "${pkgdir}/usr/bin/buzz"
  chmod u+x "${pkgdir}/usr/bin/buzz--h"
}

# $Id: PKGBUILD,v 1.12 2003/11/06 08:26:13 dorphell Exp $
# Maintainer: Marty_Stoopid <>
# Contributor: Marty_Stoopid <>
pkgname=oxymentary
pkgver=0.1
pkgrel=2
pkgdesc="Oxymentary icons theme"
arch=('any')
url="http://gnome-look.org/content/show.php?action=content&content=142007"
license=('Creative Commons by-sa')
#groups=
#provides=
#depends=()
#makedepends=()
#conflicts=()
#replaces=()
#install=
source=(http://zeroangel.overminddl1.com/misc_files/${pkgname}.tar.bz2)
md5sums=('67a7f8f7aed441cfd83e00bdf55ccfb7')
package() {
# decompress
  tar xjf ${pkgname}.tar.bz2
  rm ${srcdir}/${pkgname}/icon-theme.cache
# Install icons
  mkdir -p "${pkgdir}/usr/share/icons/${pkgname}"
  mv -T "${srcdir}/${pkgname}" "${pkgdir}/usr/share/icons/${pkgname}"
  #install -Dm644 ${srcdir}/${pkgname} "${pkgdir}/usr/share/icons/"
  
# Change the ownership to root
  chown -R root:root ${pkgdir}/*
}
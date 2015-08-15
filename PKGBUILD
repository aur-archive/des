# Maintainer: perlawk

pkgname=des
_pkgname=no_gui
pkgver=3.10
pkgrel=1
pkgdesc="The Datalog Educational System (DES) is a deductive database system with Datalog, SQL, and Relational Algebra as query languages."
url="http://des.sourceforge.net/"
arch=('i686' 'x86_64')
license=('LGPLv3')
source=( "http://downloads.sourceforge.net/project/des/des/des3.10/DES3.10Linux32SICStus.zip")
install=('des.install')

depends=('lib32-unixodbc')

build() {
  cd $srcdir/"$pkgname"
  chmod +x des
}

package() {
  cd $srcdir/"$pkgname"
  mkdir -p $pkgdir/usr/bin
  cp des $pkgdir/usr/bin
}

md5sums=('03e53de4f928895034f23943d94112f6')

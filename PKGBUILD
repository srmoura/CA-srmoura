pkgname=ca-certificates-sap
pkgver=20190215
pkgrel=1
pkgdesc="SrMoura root certificates"
arch=(any)
url="http://srmoura.com.br/"
license=('custom:Proprietary')
depends=(ca-certificates-utils)
source=('http://srmoura.com.br/CA.crt')
sha256sums=('')

package() {
  local _certdir="$pkgdir/usr/share/ca-certificates/trust-source/anchors"
  install -d "$_certdir"
  install -t "$_certdir" -m644 ./*.crt
}


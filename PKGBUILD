# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Rhys Davies <rhys@johnguant.com>

_gemname=callsign
pkgname=ruby-$_gemname
pkgver=2.2.0
pkgrel=1
pkgdesc='Look up United States Amateur (ham) Radio callsign information.'
arch=(any)
url='http://github.com/codeblock/callsign-gem'
license=()
depends=(ruby ruby-json ruby-hashie)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('f6f757297126e65412309990143ca5c06a4ccc58')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}

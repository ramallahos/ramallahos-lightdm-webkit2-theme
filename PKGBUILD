# Maintainer: Safwan Nayeem Yousuf <safwannayeemyousuf@gmail.com>
pkgname=ramallahos-lightdm-webkit2-theme
_pkgname=lightdm-webkit2-theme-glorious
pkgver=2.0.5
pkgrel=3
pkgdesc="A sleek, modern and glorified LightDM webkit2 theme"
arch=('any')
url="https://github.com/manilarome/$_pkgname"
license=('GPL3')
depends=('lightdm' 'lightdm-webkit2-greeter')
source=("$url/releases/download/v$pkgver/$_pkgname-$pkgver.tar.gz" "git+https://github.com/ramallahos/$pkgname.git")
sha512sums=('SKIP' 'SKIP')
curl https://raw.githubusercontent.com/ramallahos/$pkgname/main/lightdm.install > lightdm.install
install="lightdm.install"

package() {
	install -dm 755 "$pkgdir"/usr/share/lightdm-webkit/themes/glorious
	cp -r --no-preserve=ownership * "$pkgdir"/usr/share/lightdm-webkit/themes/glorious/
	install -Dm 644 LICENSE "$pkgdir"/usr/share/licenses/$pkgname/LICENSE
}


pkgname=namebench
pkgver=1.3.1
pkgrel=1
pkgdesc="Open-source DNS Benchmark Utility"
arch=('x86_64')
url="http://code.google.com/p/namebench/"
license=('http://www.apache.org/licenses/LICENSE-2.0')
depends=('python2')
optdepends=('tk: To enjoy GUI')
source=("https://github.com/jtrag/${pkgname}/archive/master.tar.gz")
sha512sums=('a2e0d9c90b697f5c2a940d447577287d3d80fe19c213442bbc21cfb18163ad3a2fadad4b420523d3f7859d924074f67c69dd1be1d161277fb3e898e20e91047a')

build() {
    cd "${pkgname}-master"
    python2 setup.py build 
}

package() {
    cd "${pkgname}-master"
    python2 setup.py install
}

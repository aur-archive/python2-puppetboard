
pkgname=python2-puppetboard
_realname=puppetboard
pkgver=0.0.4
pkgrel=1
pkgdesc="Web frontend for PuppetDB which relies on pypuppetdb"
arch=(any)
url="https://github.com/nedap/puppetboard"
license=("APACHE")
depends=('python2'
         'python2-flask'
         'python2-flask-wtf'
         'python2-jinja'
         'python2-markupsafe'
         'python2-wtforms'
         'python2-werkzeug'
         'python2-itsdangerous'
         'python2-requests'
         'python2-pypuppetdb')

backup=()
install=puppetboard.install
source=("http://pypi.python.org/packages/source/p/${_realname}/${_realname}-${pkgver}.tar.gz")

md5sums=('441d98db4126f7cf5c7394c8d3cd90b4')

package() {
  cd ${srcdir}/${_realname}-${pkgver}
  python2 setup.py install --root=${pkgdir}/ --optimize=1
}

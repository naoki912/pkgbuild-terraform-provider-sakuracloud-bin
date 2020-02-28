# Maintainer: Naoki Kanazawa <nk dot naoki912 at gmail dot com>
pkgname=terraform-provider-sakuracloud-bin
pkgver=2.1.1
pkgrel=1
pkgdesc="Terraform for SakuraCloud"
arch=('i686' 'x86_64')
url="https://github.com/sacloud/terraform-provider-sakuracloud"
license=('Apache')
source_x86_64=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-amd64.zip")
source_i686=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-386.zip")
sha256sums_i686=('43d9c0aa88c34d7e7c9a1c3f20d3e2747e4a5cc440dfdf19e1027308953c8f7e')
sha256sums_x86_64=('2705c41f6932b8acdcaa2ce76bb7d93a4ff4c29d76eb388b1b700f04180cd1be')


package() {
    install -d -o ${USER} -g ${USER} -m700 ${pkgdir}/${HOME}/.terraform.d/plugins/
    install -D -o ${USER} -g ${USER} -m700 "${srcdir}/terraform-provider-sakuracloud_v${pkgver}" ${pkgdir}/${HOME}/.terraform.d/plugins/
}

# Maintainer: Naoki Kanazawa <nk dot naoki912 at gmail dot com>
pkgname=terraform-provider-sakuracloud-bin
pkgver=1.20.1
pkgrel=1
pkgdesc="Terraform for SakuraCloud"
arch=('i686' 'x86_64')
url="https://github.com/sacloud/terraform-provider-sakuracloud"
license=('Apache')
source_x86_64=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-amd64.zip")
source_i686=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-386.zip")
sha256sums_i686=('cbeb539a67c47823dc5a04834ee442a82971da75a9f1ced0107f1f8205f2453b')
sha256sums_x86_64=('2d8d34a48bd33538855c5faf0bfdeaa6065a65dfa5c8b7067de219534093ef0e')


package() {
    install -d -o ${USER} -g ${USER} -m700 ${pkgdir}/${HOME}/.terraform.d/plugins/
    install -D -o ${USER} -g ${USER} -m700 "${srcdir}/terraform-provider-sakuracloud_v${pkgver}" ${pkgdir}/${HOME}/.terraform.d/plugins/
}

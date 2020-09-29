# Maintainer: Naoki Kanazawa <nk dot naoki912 at gmail dot com>
pkgname=terraform-provider-sakuracloud-bin
pkgver=2.4.1
pkgrel=1
pkgdesc="Terraform for SakuraCloud"
arch=('i686' 'x86_64')
url="https://github.com/sacloud/terraform-provider-sakuracloud"
license=('Apache')
source_x86_64=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux_amd64.zip")
source_i686=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux_386.zip")
sha256sums_i686=('0954fae8e376b2cb1a386e624933d986f61e31c3ade607501c272b4c92396dc7')
sha256sums_x86_64=('64f9b7a7fb85c03708372759c2dc5e1ed85afcbe069e89415233a091c13ced5c')


package() {
    install -d -o ${USER} -g ${USER} -m700 ${pkgdir}/${HOME}/.terraform.d/plugins/
    install -D -o ${USER} -g ${USER} -m700 "${srcdir}/terraform-provider-sakuracloud_v${pkgver}" ${pkgdir}/${HOME}/.terraform.d/plugins/
}

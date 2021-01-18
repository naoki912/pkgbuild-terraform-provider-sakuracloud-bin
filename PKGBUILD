# Maintainer: Naoki Kanazawa <nk dot naoki912 at gmail dot com>
pkgname=terraform-provider-sakuracloud-bin
pkgver=2.7.0
pkgrel=1
pkgdesc="Terraform for SakuraCloud"
arch=('i686' 'x86_64')
url="https://github.com/sacloud/terraform-provider-sakuracloud"
license=('Apache')
source_x86_64=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux_amd64.zip")
source_i686=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux_386.zip")
sha256sums_i686=('3c071f518a94316ca1ee9993d528fc4932df9e6e48543741e0978de46b00bd1c')
sha256sums_x86_64=('303422db0c16f5dcad90e60fb4a1aa95b6b5dd5cbdb505e059be112ac9c27337')


package() {
    install -d -o ${USER} -g ${USER} -m700 ${pkgdir}/${HOME}/.terraform.d/plugins/
    install -D -o ${USER} -g ${USER} -m700 "${srcdir}/terraform-provider-sakuracloud_v${pkgver}" ${pkgdir}/${HOME}/.terraform.d/plugins/
}

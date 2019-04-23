# Maintainer: Naoki Kanazawa <nk dot naoki912 at gmail dot com>
pkgname=terraform-provider-sakuracloud-bin
pkgver=1.11.4
pkgrel=1
pkgdesc="Terraform for SakuraCloud"
arch=('i686' 'x86_64')
url="https://github.com/sacloud/terraform-provider-sakuracloud"
license=('Apache')
source_x86_64=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-amd64.zip")
source_i686=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-386.zip")
sha256sums_i686=('2732c9f77b240cd42f4e66a16a4a9d187474e8f09780fc428bc36774720c73d9')
sha256sums_x86_64=('e20756fa7541381c0bceaf66e350fa4e3934c0a5a9bb74eef8740897582b28ec')


package() {
    install -d -o ${USER} -g ${USER} -m700 ${pkgdir}/${HOME}/.terraform.d/plugins/
    install -D -o ${USER} -g ${USER} -m700 "${srcdir}/terraform-provider-sakuracloud_v${pkgver}" ${pkgdir}/${HOME}/.terraform.d/plugins/
}

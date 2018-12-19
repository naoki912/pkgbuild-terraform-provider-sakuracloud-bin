# Maintainer: Naoki Kanazawa <nk dot naoki912 at gmail dot com>
pkgname=terraform-provider-sakuracloud-bin
pkgver=1.9.1
pkgrel=1
pkgdesc="Terraform for SakuraCloud"
arch=('i686' 'x86_64')
url="https://github.com/sacloud/terraform-provider-sakuracloud"
license=('Apache')
source_x86_64=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-amd64.zip")
source_i686=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-386.zip")
sha256sums_i686=('2d934e905083ddb0df9d2bb3d3f6691523b87e9fec0d66e912e8fda82976f3b3')
sha256sums_x86_64=('045495df90076e6af5e9172f44bbc5228c1520775b6e1cf6dfe5d17deb4fd82f')


package() {
    install -d -o ${USER} -g ${USER} -m755 ${pkgdir}/${HOME}/.terraform.d/plugins/
    install -D -o ${USER} -g ${USER} -m744 "${srcdir}/terraform-provider-sakuracloud_v${pkgver}_x4" ${pkgdir}/${HOME}/.terraform.d/plugins/
}

# Maintainer: Naoki Kanazawa <nk dot naoki912 at gmail dot com>
pkgname=terraform-provider-sakuracloud-bin
pkgver=1.9.0
pkgrel=1
pkgdesc="Terraform for SakuraCloud"
arch=('i686' 'x86_64')
url="https://github.com/sacloud/terraform-provider-sakuracloud"
license=('Apache')
source_x86_64=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-amd64.zip")
source_i686=("${url}/releases/download/v${pkgver}/terraform-provider-sakuracloud_${pkgver}_linux-386.zip")
sha256sums_x86_64=('e391d454aabb1c23dd977dbd68af5ae8e7b68db2cd9b1a7e8990390b224f4128')
sha256sums_i686=('a7e8533a39d2f67a4cc55861ef7401a082da6fe9f0ca4c20bd096ce0f316b05b')


package() {
    install -d -o ${USER} -g ${USER} -m755 ${pkgdir}/${HOME}/.terraform.d/plugins/
    install -D -o ${USER} -g ${USER} -m744 "${srcdir}/terraform-provider-sakuracloud_v${pkgver}_x4" ${pkgdir}/${HOME}/.terraform.d/plugins/
}

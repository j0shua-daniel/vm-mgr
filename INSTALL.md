# Install VM packages:

Debian: 
```
sudo apt-get install libvirt-clients qemu-system qemu-kvm libvirt-daemon 
```
OpenSUSE(NOT TESTED):
```
sudo zypper install libvirt qemu libvirt-daemon-driver-qemu qemu-kvm
```
Fedora(NOT TESTED):
```
sudo dnf install -y qemu-kvm libvirt virt-install bridge-utils libvirt-devel virt-top libguestfs-tools guestfs-tools
```
Arch:
```
sudo pacman -S qemu-desktop qemu-img libvirt guestfs-tools libosinfo tuned
```
Void(NOT TESTED):
```
sudo xbps-install libvirt qemu
```
Alpine:
```
doas apk add libvirt-daemon qemu-img qemu-system-x86_64 qemu-modules openrc bash
doas rc-update add libvirtd
doas service libvirtd start
doas modprobe tun
su
echo "tun" >> /etc/modules-load.d/tun.conf
cat /etc/modules | grep tun || echo tun >> /etc/modules
exit
doas addgroup $USER libvirt
doas  rc-update add libvirt-guests
doas service libvirt-guests start
```
NixOS(NOT TESTED):

ADD USER TO "libvirtd" group in /etc/nixos/configuration.nix
```nix
#in /etc/nixos/configuration.nix
virtualisation.libvirtd = {
  enable = true;
  qemu = {
    package = pkgs.qemu_kvm;
    runAsRoot = true;
    swtpm.enable = true;
    ovmf = {
      enable = true;
      packages = [(pkgs.OVMF.override {
        secureBoot = true;
        tpmSupport = true;
      }).fd];
    };
  };
};
```
Gentoo(NOT TESTED):

Please look at the [wiki](https://wiki.gentoo.org/wiki/QEMU)
```
sudo emerge --ask app-emulation/qemu
```
Slackware(NOT TESTESD):

[Read and follow instructions.](https://docs.slackware.com/howtos:general_admin:kvm_libvirt)

Freebsd:
```
NOT SUPPORTED
```
NetBSD:
```
NOT SUPPORTED
```

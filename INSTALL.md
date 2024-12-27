# Install VM packages:

Debian: 
```
sudo apt-get install libvirt-clients qemu-system qemu-kvm libvirt-daemon 
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
Freebsd:
```
NOT SUPPORTED
```
NetBSD:
```
NOT SUPPORTED
```

# Install KVM and qemu:
THIS HAS ONLY BEEN TESTED ON ALPINE!

On Debian: 
```
sudo apt-get install libvirt-clients qemu-system qemu-kvm libvirt-daemon 
```
On Fedora:
```
sudo dnf install -y qemu-kvm libvirt virt-install bridge-utils libvirt-devel virt-top libguestfs-tools guestfs-tools
```
On Arch:
```
sudo pacman -S qemu-all qemu-img libvirt guestfs-tools libosinfo tuned
```
On Void:
```
sudo xbps-install libvirt qemu polkit
```
On Alpine:
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



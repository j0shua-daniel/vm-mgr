# VM Manager
A set of bash scripts to make using qemu a breeze.

See the [Gallery](https://github.com/j0shua-daniel/vm-manager/blob/main/gallery.md)

## Install:
NOT TESTED ON FEDORA & VOID LINUX!

For Linux:
[Install KVM & qemu](https://github.com/j0shua-daniel/vm-manager/blob/main/INSTALL.md)

For FreeBSD
[Install bhyve](https://github.com/j0shua-daniel/vm-manager/blob/main/INSTALL.md)

For NetBSD
[Install NVMM](https://github.com/j0shua-daniel/vm-manager/blob/main/INSTALL.md)

```
git clone https://github.com/j0shua-daniel/vm-manager
cd vm-manager
chmod +x setup
./setup
```

## Creating a vm:
REMEMBER: When setting ram & disk size end the number with G or M. So when setting ram don't do "3000" do "3000M".

```
vm-manager 
```
You will see this: 
```
1) Start a VM
2) Create a VM
3) Delete a VM
4) Quit
Please enter your choice:
```
Type "2" to create your first vm!

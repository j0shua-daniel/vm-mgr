# VM Manager
A set of bash scripts to make using qemu a breeze.

## Install:
Make sure you have qemu and kvm installed!

```
git clone https://github.com/j0shua-daniel/vm-manager
cd vm-manager
chmod +x create-vm launch-vm delete-vm vm-manager
sudo  mv launch-vm delete-vm vm-manager /usr/bin/
```

## Creating a vm:

```
vm-manager 
```
You will see this: 
```
1) Launch a VM
2) Create a VM
3) Delete a VM
4) Quit
Please enter your choice:
```
Type "2" to create your first vm!

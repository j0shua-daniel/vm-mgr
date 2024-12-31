# Virtual Machine Manager
A set of minimal bash scripts to simplify and hasten the process of making virtual machines. 

Virtual Machine with 255 threads, on a 12 thread computer!

![255th](https://github.com/j0shua-daniel/images/blob/main/255cores.png?raw=true)

## Install:

Run `alias "sudo"="doas"` in your terminal if you use `doas`. 

[Install & Setup VM packages](https://github.com/j0shua-daniel/vm-mgr/wiki)

```
git clone https://github.com/j0shua-daniel/vm-mgr
cd vm-mgr
chmod +x setup
./setup
```

## Usage:
Here is a [video](https://github.com/j0shua-daniel/images/blob/main/vm-mgr.gif) (it is a little broken).

Type "4" to get the help script, read through it carefully, if there are any problems open an issue.

```
vm-mgr
```
You will see this: 
```
1) Start a VM
2) Create a VM
3) Delete a VM
4) Help
5) Quit
Option:
```
Type "2" to create your first vm!

## Compaired to alternatives.

1. vm-mgr is more easy to use than just qemu.
2. vm-mgr allows set ram to be below 64MB unlike virt-manager & gnome-boxes.
3. vm-mgr allows cpu threads up to 255, while on others (bar qemu itself) you can only go up to what is on your pc.
4. vm-mgr is cli unlike virt-manager, gnome-boxes, virtualbox and cockpit.
5. vm-mgr is **planning** to have support for BSD unlike gnomeboxes.

## Todo:

- [ ] Add BSD support.
- [x] Make menus more clear.
- [x] Fix bugs.
- [ ] Bridge the network.
- [ ] Enable starting created vms without disks and only isos/imgs.
- [x] Add *.img support.


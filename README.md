# Virtual Machine Manager
A set of minimal bash scripts to simplify and hasten the process of making virtual machines. 

Virtual Machines with 255 threads, on a 12 thread computer!

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
Here is a [video](https://github.com/j0shua-daniel/images/blob/main/vm-mgr.gif).

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

## Todo:

- [ ] Add BSD support.
- [x] Make menus more clear.
- [x] Fix bugs.
- [ ] Bridge the network.
- [ ] Enable starting created vms without disks and only isos/imgs.


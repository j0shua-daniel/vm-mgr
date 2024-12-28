# Virtual Machine Manager
A set of minimal bash scripts to simplify and hasten the process of making virtual machines. 

The [gallery.](https://github.com/j0shua-daniel/vm-mgr/blob/main/gallery.md)

## Install:

For those using doas do run `alias "sudo"="doas"` in your terminal. 

Not tested on void & fedora. 

[NO SUPPORT FOR BSD YET!](https://github.com/j0shua-daniel/vm-mgr/blob/main/bsd.md)

[Install & Setup VM packages](https://github.com/j0shua-daniel/vm-mgr/blob/main/INSTALL.md)


```
git clone https://github.com/j0shua-daniel/vm-mgr
cd vm-mgr
chmod +x setup
./setup
```

## Usage:
Here is a [video](https://github.com/j0shua-daniel/images/blob/main/2024-12-28%2008-37-41.mp4) (requires a download!)

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
## Uninstall:
```
git clone https://github.com/j0shua-daniel/vm-mgr
cd vm-mgr
chmod +x remove-vm-mgr
sudo ./remove-vm-mgr
```
## About:
This project is something I have been wanting to do for a very long time, I always find VM software always a bit glitchy, sometimes too simple and even too complex. These scripts are made to ensure speed and simplicity. Yes they won't be flawless (there are going to be glitches!). Also I found that VM software on BSD is very difficult and that is why im planning to add BSD support soon! 

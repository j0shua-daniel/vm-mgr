# Virtual Machine Manager

[Website](https://coalition-friends-affairs-wages.trycloudflare.com) & [Wiki](https://coalition-friends-affairs-wages.trycloudflare.com/wiki/)

<a href="https://coalition-friends-affairs-wages.trycloudflare.com/">
<p align="center" width="100%">
    <img width="270px" src="https://github.com/j0shua-daniel/images/blob/main/favcon.png?raw=true"> 
</p>
</a>

<p align="center" ">Blazing fast VM manager, that just works.</p>


## Install:

To install vm-mgr, run:

```
curl -s https://raw.githubusercontent.com/j0shua-daniel/vm-mgr/refs/heads/main/setup | bash
```

Distros supported by the installer:

1. Debian/Debian based.
2. Arch/Arch based.
3. OpenSUSE.
4. RHEL/Fedora/RHEL based.
5. Alpine.
6. Void.
7. ~~Nixos~~ (comming soon!)
8. ~~Gentoo~~ (comming soon!)
9. ~~Solus~~ (comming soon!)
10. ~~Slackware~~ (comming soon!)
11. Clear Linux.
12. Fedora Silverblue (inside fedora toolbox).
    
If your distro is not supported by the installer please refer to the [wiki](https://github.com/j0shua-daniel/vm-mgr/wiki).

## Usage:

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

## Cool Features.
1. Minimal - vm-mgr is cli based, meaning it uses as little resources as possible!
2. Can run VM's with less than 64MB ram. - Some other VM managers set the min memory for a VM to 64MB!
3. Can run VM's with more threads. - Some other VM managers set the max threads to what the host has.
4. It uses the terminal. - Makes the terminal even more powerful.
5. BSD support - vm-mgr **plans** to add BSD support!

## Todo:

- [ ] Add BSD support.
- [x] Make menus more clear.
- [x] Fix bugs.
- [ ] Bridge the network.
- [ ] Enable starting created vms without disks and only isos/imgs.
- [x] Add *.img support.


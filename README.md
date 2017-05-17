# Virsh Utilities
A couple of utilities to simplify basic operations with `virsh` on multiple domains

## Vstart

### Usage
This script can work in two ways:
* With no arguments will list all domains managed by `virsh` and their status.
```sh
vstart
```
* With a list of the domains to start.
```sh
vstart domain1 domain2 domain3 ...
```
### Output
The scripts outputs one line per domain giving the status of the operation.


## Vstop

### Usage
This script accepts three `virsh` arguments that will be applied to all running domains.
* `shutdown` This is the default argument and can be obviated
* `destroy`
* `reboot`
Any other argument will show the script's help.

### Output
The script outputs one line per domain with the same output as `virsh`.


# Why I created this?
I have been studying for the RHCSA exam so I had to create many different VMs during the process, sometimes I had 5 VMs working at the same time. Every time I had to turn them off it was a big burden to make them stop nicely so I came up with the idea of creating this script. Also it was very helpful to learn more about bash programming, it couldn't be better.

So if you are in the same situation as I was with plenty of VMs running this might be helpful to you too. So please enjoy it.

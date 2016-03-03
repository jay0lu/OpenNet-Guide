# Installation Guide for OpenNet


---

OpenNet is an open source Software-Defined Wireless Local Area Network (SDWLAN) simulator which connects Mininet to ns-3 to support both SND controller compatibility and wireless/mobility modelling.

---
## Install Ubuntu

OpenNet is based on Mininet, you need a Linux environment to run it.

If your computer doesn't have Linux OS, you can download and install the following virtualization systems to run Linux on your computer:
>* I recommend [VirtualBox](https://www.virtualbox.org/wiki/Downloads) 
>*  [VMware Workstation](http://www.vmware.com/products/workstation/)

Then download [Ubuntu 14.04 LTS](http://www.ubuntu.com/download/desktop) and install it in your virtual machine.

---
In Ubuntu terminal, follow those steps:
```
$ sudo su -
# cd OpenNet
# git clone https://github.com/noxrepo/pox.git
# cd OpenNet/pox
# ./pox.py forwarding.l2_learning &
# cd OpenNet/mininet/examples/opennet
```

(In terminal, $ means your are regular user permission, # means your are in root permission. Be careful when you are in root permission!)

```
# python wifiroaming.py
```
Do not add sudo to run the example, you are alreadly in root permission. 

If the example cannot connect to the controller, you may try to stop the netwok-manager.
```
# service network-manager stop
```

Here is the command to restart the network-manager.
```
# service network-manager start
```

---
## Reference
[OpenNet](https://github.com/dlinknctu/OpenNet)





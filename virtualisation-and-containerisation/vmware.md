## VMWare

### VMWare Workstation

#### To Update Kernel Modules

After updating a Linux kernel, the following command will re-compile all the VMWare kernel modules to match the new kernel.

`sudo /usr/bin/vmware-modconfig --console --install-all`
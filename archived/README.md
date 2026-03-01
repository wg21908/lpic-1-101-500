# LPIC-1 : 101-500 Cheat Sheet

|Question|Answer|
|--------------------|--------------------|
|What is /sys?|/sys is a virtual filesystem called sysfs.|
|What does sysfs provide|Kernel objects, Devices, Drivers, Bus types, & Hardware information|
|Is sysft a real disk filesystem|No — it is created dynamically by the kernel at runtime.
|How /sys is mounted|sysfs on /sys type sysfs (rw,nosuid,nodev,noexec,relatime)| 
|Does /sys exist only in memory|Yes|
|Is /sys populated by the kernel|Yes|
|Does /sys expose kernel and device info as files and directories|Yes|
|Is /sys usually mounted automatically at boot?|Yes|
|/proc and /sys comparisions|/proc is process-oriented where-as /sys is device-oriented|
|/proc and /sys comparisions|/proc has an older interface where-as /sys has a newer, structured interface|
|/proc and /sys comparisions|/proc things are located at /proc/cpuinfo etc, where-as /sys things are at /sys/devices/...|
|/proc and /sys comparisions|/proc has mixed info where-as /sys is a clean hardware model|
|Which filesystem provides structured hardware and driver information?|/sys|
|Where are block devices?|ls /sys/block, Ex: sda, sdb, nvme0n1, loop0|
|What does /sys/class show?|/sys/class shows logical device groupings.<br />Ex: ls /sys/class/net, displays eth0, lo, wlan0| 
|What does /sys/bus represent?|Represents hardware buses.<br />Ex: ls /sys/bus/pci/devices|
|Can You Modify Things in /sys?|Yes — some files are writable.|
|Which virtual filesystem provides a hierarchical view of kernel devices?|/sys|
|Which directory contains block device information exposed by the kernel?|/sys/block|
|What type of filesystem is /sys?|Virtual filesystem (sysfs)|
|What is lsusb?|Lists USB (Universal Serial Bus) devices currently connected to the machine.|<br />the USB interface is largely used to connect input devices — keyboards, pointing devices — and removable storage media|
|Where does lsusb read data from?|/sys/bus/usb and /proc/bus/usb|
|What does lsusb show?|All connected USB devices, Vendor ID, Product ID, Device description, Bus number and device number<br />For lsusb, `Bus 002 Device 003: ID 046d:c534 Logitech, Inc.`|
|Show lsusb with verbosity|lsusb -v|
|Show lsusb in tree view|lsusb -t|
|Show a specifiy bus/device|lsusb -s 002:003|
|Show a vendor:product filter w/lsusb|lsusb -d 046d:c534|



    /proc/
    /dev/
    modprobe
    lsmod
    lspci
    

    Enable and disable integrated peripherals.
    Differentiate between the various types of mass storage devices.
    Determine hardware resources for devices.
    Tools and utilities to list various hardware information (e.g. lsusb, lspci, etc.).
    Tools and utilities to manipulate USB devices.
    Conceptual understanding of sysfs, udev and dbus.









## Topic 101.2: System Architecture - Boot the system
## Topic 101.3: System Architecture - Change runlevels / boot targets and shutdown or reboot system 
## Topic 102.1: Linux Installation and Package Management
## Topic 102.2: Linux Installation and Package Management
## Topic 102.3: Linux Installation and Package Management
## Topic 102.4: Linux Installation and Package Management
## Topic 102.5: Linux Installation and Package Management
## Topic 102.6: Linux Installation and Package Management
## Topic 103.1: GNU and Unix Commands
## Topic 103.2: GNU and Unix Commands
## Topic 103.3: GNU and Unix Commands
## Topic 103.4: GNU and Unix Commands
## Topic 103.5: GNU and Unix Commands
## Topic 103.6: GNU and Unix Commands
## Topic 103.7: GNU and Unix Commands
## Topic 103.8: GNU and Unix Commands
## Topic 104.1: Devices, Linux Filesystems, Filesystem Hierarchy Standard
## Topic 104.2: Devices, Linux Filesystems, Filesystem Hierarchy Standard
## Topic 104.3: Devices, Linux Filesystems, Filesystem Hierarchy Standard
## Topic 104.4: Devices, Linux Filesystems, Filesystem Hierarchy Standard
## Topic 104.5: Devices, Linux Filesystems, Filesystem Hierarchy Standard
## Topic 104.6: Devices, Linux Filesystems, Filesystem Hierarchy Standard
## Topic 104.7: Devices, Linux Filesystems, Filesystem Hierarchy Standard

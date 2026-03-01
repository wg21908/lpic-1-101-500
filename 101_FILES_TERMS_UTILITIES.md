# Files, Terms & Utilities

System Architecture

[Back](README.md)

## Topic 101

| Category | Item     | Definition | Purpose |
|----------|----------|------------|----------|
| File | /sys/ | Virtual filesystem (sysfs) exposing kernel device and driver information. | Used to view and interact with kernel-managed device data and attributes. |
| File | /proc/ | Virtual filesystem providing process and kernel information. | Used to inspect system status, processes, and kernel parameters. |
| File | /dev/ | Directory containing device files representing hardware and virtual devices. | Provides user-space access to hardware devices. |
| Utility | modprobe | Command used to add or remove Linux kernel modules. | Loads or unloads kernel modules along with their dependencies. |
| Utility | lsmod | Command that displays currently loaded kernel modules. | Used to verify which kernel modules are active. |
| Utility | lspci | Command that lists devices connected to the PCI bus. | Used to inspect PCI hardware devices. |
| Utility | lsusb | Command that lists devices connected to the USB bus. | Used to inspect USB hardware devices. |
| Utility | dmesg | Command that displays kernel ring buffer messages. | Used to view kernel boot messages and hardware-related events. |
| Utility | journalctl | Command used to query and display logs from the systemd journal. | Used to inspect system and service logs. |
| Term | BIOS | Basic Input/Output System; legacy firmware interface for initializing hardware during boot. | Initializes hardware and starts the boot process on older systems. |
| Term | UEFI | Unified Extensible Firmware Interface; modern firmware replacing BIOS. | Initializes hardware and loads bootloaders on modern systems. |
| Term | bootloader | Program that loads the operating system kernel into memory. | Transfers control from firmware to the kernel. |
| Term | kernel | Core component of the operating system managing hardware and system resources. | Controls CPU, memory, devices, and provides system services. |
| Term | initramfs | Initial RAM filesystem loaded temporarily during boot. | Provides necessary drivers and tools needed to mount the real root filesystem. |
| Term | init | First process started by the kernel (PID 1). | Initializes user space and starts system services. |
| Term | SysVinit | Traditional Unix System V init system based on runlevels. | Manages system services using runlevels and startup scripts. |
| Term | systemd | Modern init system and service manager for Linux systems. | Initializes the system and manages services, units, and logging. |
| File | /etc/inittab | Configuration file used by SysVinit to define default runlevel and system initialization behavior. | Controls system runlevels and startup processes in SysVinit systems. |
| Utility | shutdown | Command used to safely power off or reboot the system. | Shuts down or restarts the system in a controlled manner. |
| Utility | init | Program that initializes the system and becomes process ID 1. | Starts and manages system services during boot. |
| Directory | /etc/init.d/ | Directory containing SysVinit service scripts. | Stores startup and shutdown scripts for system services. |
| Utility | telinit | Command used to change the system runlevel. | Switches between runlevels in SysVinit systems. |
| Term | systemd | Modern init system and service manager replacing SysVinit on most Linux systems. | Manages system initialization, services, and system state. |
| Utility | systemctl | Command-line tool to control and manage systemd services and units. | Starts, stops, enables, disables, and queries system services. |
| Directory | /etc/systemd/ | Directory containing systemd configuration files and overrides. | Stores administrator-defined unit files and configuration changes. |
| Directory | /usr/lib/systemd/ | Directory containing systemd unit files provided by installed packages. | Stores default systemd service unit definitions. |

[Back](README.md)

# Files, Terms & Utilities

System Architecture

[Back](README.md)

## Topic 101

| Category | Item     | Definition | Purpose |
|----------|----------|------------|----------|
| Command | lsusb | Lists USB buses and devices connected to the system. | Used to identify and troubleshoot USB hardware. |
| Command | lspci | Lists PCI buses and attached devices. | Used to inspect PCI devices such as GPUs and network cards. |
| Command | lsmod | Displays currently loaded kernel modules. | Used to verify which drivers are active in the running kernel. |
| Command | modprobe | Loads or removes kernel modules with dependency handling. | Used to manage kernel modules safely with automatic dependency resolution. |
| Command | rmmod | Removes a loaded kernel module from the kernel. | Used to manually unload a module. |
| Command | insmod | Inserts a kernel module into the running kernel without resolving dependencies. | Used for manual module loading. |
| Command | modinfo | Displays information about a kernel module. | Used to view module metadata, parameters, and dependencies. |
| Command | depmod | Generates kernel module dependency files. | Used to prepare module dependency maps for modprobe. |
| Command | uname | Displays system and kernel information. | Used to determine kernel version and system details. |
| Command | arch | Displays the system's CPU architecture. | Used to verify hardware architecture (e.g., x86_64). |
| Command | free | Displays memory usage statistics. | Used to monitor RAM and swap usage. |
| Command | cat | Displays file contents. | Used to view files including virtual files under /proc and /sys. |
| Command | grep | Searches for patterns in text using regular expressions. | Used to filter command output or search within files. |
| Command | watch | Repeatedly runs a command and displays updated output. | Used to monitor system changes in real time. |
| Command | hwinfo | Displays detailed hardware information. | Used to obtain comprehensive system hardware data. |
| Virtual File | /proc/cpuinfo | Virtual file containing CPU details and flags. | Used to inspect CPU model, features, and vulnerabilities. |
| Virtual File | /proc/meminfo | Virtual file showing memory statistics. | Used to check RAM and swap usage details. |
| Virtual File | /proc/modules | Lists currently loaded kernel modules. | Used to verify active kernel modules. |
| Virtual File | /proc/interrupts | Displays interrupt (IRQ) usage by devices. | Used to analyze hardware interrupt assignments. |
| Virtual File | /proc/ioports | Lists I/O port allocations. | Used to inspect device I/O port usage. |
| Virtual File | /proc/filesystems | Lists supported filesystems by the kernel. | Used to verify available filesystem support. |
| Virtual Directory | /sys/ | Virtual filesystem (sysfs) exposing kernel device and driver data. | Used to interact with kernel-managed devices. |
| Virtual Directory | /sys/class/ | Contains device class information in sysfs. | Used to view devices grouped by class (e.g., network, block). |
| Virtual Directory | /sys/block/ | Contains block device information. | Used to inspect disks and storage devices. |
| Directory | /dev/ | Directory containing device files. | Used to access hardware devices via special files. |
| Device File | /dev/sda | First detected SATA/SCSI disk device. | Used to access primary storage device. |
| Device File | /dev/sdb | Second detected SATA/SCSI disk device. | Used to access additional storage devices. |
| Device File | /dev/nvme0n1 | First NVMe storage device. | Used to access NVMe SSDs. |
| Device File | /dev/tty* | Terminal interface devices. | Used for terminal and console communication. |
| Device File | /dev/null | Special device that discards all written data. | Used to suppress unwanted output. |
| Device File | /dev/zero | Special device providing infinite null bytes. | Used to create empty data streams. |
| Device File | /dev/random | Provides blocking random data from kernel entropy pool. | Used for cryptographic randomness. |
| Device File | /dev/urandom | Provides non-blocking random data. | Used for general-purpose randomness. |
| Directory | /lib/modules/$(uname -r)/ | Contains kernel modules for the running kernel version. | Used to store and manage loadable kernel modules. |
| Config File | /etc/modprobe.conf | Configuration file for modprobe (legacy systems). | Used to configure module options and aliases. |
| Directory | /etc/modprobe.d/ | Directory containing modprobe configuration files. | Used to configure module behavior and blacklist modules. |
| Hardware Concept | PCI | Peripheral Component Interconnect bus standard. | Used to connect expansion hardware like GPUs and NICs. |
| Hardware Concept | USB | Universal Serial Bus interface standard. | Used to connect external peripherals. |
| Hardware Concept | SATA | Serial ATA storage interface standard. | Used to connect hard drives and SSDs. |
| Hardware Concept | IRQ | Interrupt Request line used by hardware devices. | Used by devices to signal the CPU for attention. |
| Hardware Concept | DMA | Direct Memory Access mechanism. | Allows hardware to access memory without CPU intervention. |
| Hardware Concept | I/O Ports | Hardware communication addresses for devices. | Used for low-level device communication. |
| Hardware Concept | Block Device | Device that transfers data in fixed-size blocks. | Used for storage devices like disks. |
| Hardware Concept | Character Device | Device that transfers data character by character. | Used for devices like terminals and serial ports. |
| Hardware Concept | Major/Minor Numbers | Numerical identifiers for device drivers and devices. | Used by the kernel to map device files to drivers. |
| System Component | udev | Device manager for the Linux kernel. | Dynamically manages device nodes in /dev. |

[Back](README.md)

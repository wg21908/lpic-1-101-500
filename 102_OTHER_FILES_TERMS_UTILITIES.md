# Files, Terms & Utilities

Linux Installation and Package Management

[Back](README.md)

## Topic 102

| Category | Item       | Definition                                                 | Purpose                                     |
| -------- | ---------- | ---------------------------------------------------------- | ------------------------------------------- |
| Utility   | fdisk                | Command-line partition table editor for MBR and GPT disks. | Create, delete, and modify disk partitions. |
| Utility   | cfdisk               | Text-based partition editor.                               | Interactive disk partition management.      |
| Utility   | parted               | Advanced partitioning tool supporting large disks and GPT. | Create, resize, and manage partitions.      |
| Utility   | mkfs                 | Creates a filesystem on a partition.                       | Format partitions for use.                  |
| Utility   | mkfs.ext4            | Creates an ext4 filesystem.                                | Format partition as ext4.                   |
| Utility   | mkswap               | Initializes a partition or file for swap usage.            | Prepare swap space.                         |
| Utility   | swapon               | Enables swap space.                                        | Activate swap.                              |
| Utility   | swapoff              | Disables swap space.                                       | Deactivate swap.                            |
| File      | /etc/fstab           | Static filesystem mount configuration file.                | Defines filesystems mounted at boot.        |
| Utility   | mount                | Attaches a filesystem to a directory.                      | Make filesystem accessible.                 |
| Utility   | umount               | Detaches a mounted filesystem.                             | Safely remove filesystem access.            |
| Utility   | blkid                | Displays block device attributes including UUID.           | Identify filesystems and UUIDs.             |
| Term      | UUID                 | Unique identifier assigned to a filesystem.                | Stable reference for mounting.              |
| Term      | LABEL                | Human-readable filesystem label.                           | Alternative mount reference.                |
| Term      | ext4                 | Journaling Linux filesystem.                               | Store files reliably with recovery support. |
| Term      | XFS                  | High-performance journaling filesystem.                    | Used in enterprise storage.                 |
| Term      | Btrfs                | Advanced Linux filesystem with snapshot support.           | Modern filesystem with advanced features.   |
| Term      | inode                | Metadata structure describing a file.                      | Stores file attributes and block pointers.  |
| Term      | journaling           | Filesystem feature that logs changes before writing.       | Improves crash recovery.                    |
| Term      | LVM                  | Logical Volume Manager abstraction layer.                  | Flexible disk management and resizing.      |
| File      | /boot/grub/grub.cfg  | GRUB 2 configuration file (Debian-based).                  | Defines boot menu entries.                  |
| File      | /boot/grub2/grub.cfg | GRUB 2 configuration file (RPM-based).                     | Defines boot entries.                       |
| File      | /etc/default/grub    | GRUB default settings file.                                | Controls timeout and kernel parameters.     |
| Utility   | update-grub          | Debian command to regenerate GRUB config.                  | Refresh grub.cfg.                           |
| Term      | GPT                  | GUID Partition Table format.                               | Modern partitioning scheme.                 |
| Term      | EFI System Partition | FAT32 partition used by UEFI firmware.                     | Stores EFI bootloaders.                     |
| Term      | initramfs            | Initial RAM filesystem loaded during boot.                 | Loads drivers before mounting root.         |
| Utility   | dracut               | Creates initramfs image.                                   | Generate initial boot image.                |
| Term      | kernel parameters    | Boot-time options passed to kernel.                        | Modify system startup behavior.             |
| Term      | chainloading         | Booting another OS from GRUB.                              | Support multi-boot setups.                  |
| File      | /etc/ld.so.cache     | Compiled cache of shared libraries.                        | Speed up dynamic linking.                   |
| Directory | /lib                 | Essential shared libraries.                                | Required for system boot and core programs. |
| Directory | /usr/lib             | Non-essential shared libraries.                            | Libraries for user applications.            |
| Term      | SONAME               | Embedded shared object name inside library.                | Version compatibility management.           |
| Term      | dynamic linking      | Libraries linked at runtime.                               | Reduce executable size.                     |
| Term      | static linking       | Libraries compiled into executable.                        | No runtime library dependency.              |
| Utility   | dpkg -i              | Installs a .deb package file.                              | Manual package installation.                |
| Utility   | dpkg -r              | Removes installed package.                                 | Uninstall package.                          |
| Utility   | dpkg -l              | Lists installed packages.                                  | Query installed software.                   |
| Utility   | apt                  | Modern Debian package management frontend.                 | Simplified package management.              |
| Utility   | apt update           | Updates repository package lists.                          | Refresh metadata.                           |
| Utility   | apt upgrade          | Upgrades installed packages.                               | Apply updates.                              |
| Utility   | apt remove           | Removes a package.                                         | Uninstall software.                         |
| Utility   | apt purge            | Removes package and config files.                          | Full removal.                               |
| Utility   | apt search           | Searches package repositories.                             | Locate packages.                            |
| File      | /var/lib/dpkg/status | Database of installed packages.                            | Track installation state.                   |
| Term      | dependency           | Required supporting package.                               | Ensure software functions correctly.        |
| Term      | repository           | Centralized package source server.                         | Provide installable software.               |
| Utility   | rpm -ivh             | Installs RPM package file.                                 | Install software manually.                  |
| Utility   | rpm -e               | Removes RPM package.                                       | Uninstall software.                         |
| Utility   | rpm -qa              | Lists installed RPM packages.                              | Query system packages.                      |
| Utility   | dnf                  | Modern replacement for yum.                                | Improved package management.                |
| Utility   | dnf install          | Installs package via DNF.                                  | Install software with dependencies.         |
| Utility   | dnf remove           | Removes package.                                           | Uninstall software.                         |
| Utility   | dnf update           | Updates installed packages.                                | Apply system updates.                       |
| Directory | /var/lib/rpm/        | RPM database location.                                     | Track installed packages.                   |
| Term      | GPG signature        | Cryptographic package verification method.                 | Ensure package authenticity.                |
| Term      | hypervisor           | Software managing virtual machines.                        | Enable virtualization.                      |
| Term      | Type 1 hypervisor    | Bare-metal hypervisor running directly on hardware.        | Enterprise virtualization.                  |
| Term      | Type 2 hypervisor    | Hypervisor running on host OS.                             | Desktop virtualization.                     |
| Term      | KVM                  | Kernel-based Virtual Machine technology.                   | Linux-native virtualization.                |
| Term      | QEMU                 | Emulator and virtual machine monitor.                      | Hardware emulation and VM support.          |
| Term      | virtio               | Paravirtualized device drivers.                            | Improve VM performance.                     |
| Term      | cloud-init           | Tool for VM initialization at first boot.                  | Automate configuration.                     |
| Term      | namespaces           | Kernel feature isolating processes.                        | Container process separation.               |
| Term      | cgroups              | Kernel feature limiting resource usage.                    | Control CPU and memory allocation.          |

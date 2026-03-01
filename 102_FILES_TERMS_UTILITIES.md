# Files, Terms & Utilities

Linux Installation and Package Management

[Back](README.md)

## Topic 102

| Category | Item | Definition | Purpose |
|----------|------|------------|----------|
| Filesystem | / (root) filesystem | The top-level filesystem containing the entire directory hierarchy. | Provides the base structure of the operating system and contains essential system files. |
| Filesystem | /var filesystem | A filesystem containing variable data such as logs, spool files, and caches. | Stores data that changes frequently during system operation. |
| Filesystem | /home filesystem | A filesystem containing user home directories. | Stores personal user data and configuration files. |
| Filesystem | /boot filesystem | A filesystem containing bootloader files, kernel images, and related boot files. | Required for system startup and kernel loading. |
| Filesystem | EFI System Partition (ESP) | A special FAT32 partition used by UEFI firmware to store bootloaders and EFI applications. | Allows UEFI systems to locate and execute bootloaders. |
| Concept | swap space | Disk space used as virtual memory when physical RAM is exhausted. | Extends available memory and supports memory management. |
| Concept | mount points | Directories where filesystems are attached to the directory tree. | Provide access to filesystems within the unified directory hierarchy. |
| Concept | partitions | Logical divisions of a storage device. | Allow separation of data, operating systems, or filesystems on a single physical disk. |
| File | menu.lst, grub.cfg, grub.conf | Configuration files used by GRUB (Legacy and GRUB 2). | Define boot menu entries and bootloader settings. |
| Utility | grub-install | Command used to install the GRUB bootloader to a device. | Writes GRUB to the MBR or EFI System Partition. |
| Utility | grub-mkconfig | Command used to generate a GRUB 2 configuration file. | Automatically builds grub.cfg based on system configuration. |
| Term | MBR | Master Boot Record; first sector of a disk containing bootloader code and partition table. | Initiates boot process on BIOS-based systems. |
| Utility | ldd | Command that lists shared library dependencies of an executable. | Identifies required shared libraries for a program. |
| Utility | ldconfig | Command that updates the system's shared library cache. | Refreshes linker cache after adding or modifying libraries. |
| File | /etc/ld.so.conf | Configuration file listing library search paths for the dynamic linker. | Defines additional directories for shared libraries. |
| Term | LD_LIBRARY_PATH | Environment variable specifying additional library search paths. | Temporarily overrides shared library search locations. |
| File | /etc/apt/sources.list | Configuration file defining APT package repositories. | Specifies software sources for package installation and updates. |
| Utility | dpkg | Debian package management tool. | Installs, removes, and queries .deb packages. |
| Utility | dpkg-reconfigure | Command to reconfigure an installed Debian package. | Re-runs package configuration scripts. |
| Utility | apt-get | APT command-line package management tool. | Installs, removes, and upgrades packages with dependency resolution. |
| Utility | apt-cache | APT command to query package information. | Displays metadata about packages and repositories. |
| Utility | rpm | Red Hat Package Manager tool. | Installs, removes, and queries .rpm packages. |
| Utility | rpm2cpio | Utility that converts an RPM package into a cpio archive. | Extracts files from an RPM without installing it. |
| File | /etc/yum.conf | Configuration file for YUM package manager. | Defines global YUM settings. |
| Directory | /etc/yum.repos.d/ | Directory containing repository configuration files for YUM/DNF. | Stores .repo files defining software repositories. |
| Utility | yum | Package management tool for RPM-based systems. | Installs, removes, and updates packages with dependency resolution. |
| Utility | zypper | Package management tool used in SUSE-based systems. | Manages software packages and repositories. |
| Term | Virtual machine | Software-based emulation of a physical computer system. | Runs multiple operating systems on a single physical host. |
| Term | Linux container | OS-level virtualization method using shared kernel. | Isolates applications while sharing the host kernel. |
| Term | Application container | Container packaging an application and its dependencies. | Ensures consistent application deployment across environments. |
| Term | Guest drivers | Drivers installed inside a virtual machine optimized for the hypervisor. | Improve performance and integration with host system. |
| File | SSH host keys | Cryptographic keys identifying an SSH server. | Provide server authentication and secure connections. |
| File | D-Bus machine id | Unique identifier stored on a Linux system for D-Bus messaging. | Distinguishes systems and supports inter-process communication. |

[Back](README.md)

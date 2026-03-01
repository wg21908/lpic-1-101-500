# Files, Terms & Utilities

System Architecture

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

[Back](README.md)

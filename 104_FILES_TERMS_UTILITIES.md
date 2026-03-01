# Files, Terms & Utilities

Devices, Linux Filesystems, Filesystem Hierarchy Standard

[Back](README.md)

## Topic 104

| Category | Item | Definition | Purpose |
|----------|------|------------|----------|
| Utility | fdisk | Command-line partition editor for MBR (and limited GPT) partition tables. | Creates, deletes, and modifies disk partitions on storage devices. |
| Utility | gdisk | GPT fdisk; a partitioning tool specifically for GPT partition tables. | Creates, deletes, and manages GPT partitions on disks. |
| Utility | parted | GNU partition manipulation program supporting MBR and GPT. | Used to create, resize, delete, and inspect partitions. |
| Utility | mkfs | Command used to create a filesystem on a partition or device. | Formats a partition with a specified filesystem type (e.g., ext4, xfs). |
| Utility | mkswap | Command used to set up a swap area on a device or file. | Initializes a partition or file to be used as swap space. |
| Utility | du | Disk usage command. | Estimates file and directory space usage. |
| Utility | df | Disk free command. | Reports filesystem disk space usage. |
| Utility | fsck | Filesystem consistency check utility. | Checks and repairs filesystems. |
| Utility | e2fsck | ext2/3/4 filesystem check utility. | Checks and repairs ext-based filesystems. |
| Utility | mke2fs | Creates an ext2/3/4 filesystem. | Formats a partition with an ext filesystem. |
| Utility | tune2fs | Adjusts tunable parameters of ext2/3/4 filesystems. | Modifies filesystem settings without reformatting. |
| Utility | xfs_repair | Repairs XFS filesystems. | Checks and fixes XFS filesystem errors. |
| Utility | xfs_fsr | XFS filesystem reorganizer. | Defragments XFS filesystems. |
| Utility | xfs_db | XFS filesystem debugger. | Examines and debugs XFS filesystem structures. |
| File | /etc/fstab | Filesystem table configuration file. | Defines filesystems and mount options used during system boot. |
| Directory | /media/ | Directory typically used for removable media mount points. | Provides mount locations for USB drives, CDs, and other removable devices. |
| Utility | mount | Command used to attach a filesystem to the directory tree. | Mounts filesystems manually or displays mounted filesystems. |
| Utility | umount | Command used to detach a mounted filesystem. | Unmounts filesystems safely from the directory tree. |
| Utility | blkid | Command that displays block device attributes. | Shows UUID, filesystem type, and label information for devices. |
| Utility | lsblk | Command that lists block devices in a tree format. | Displays disk, partition, and mount point relationships. |
| Utility | chmod | Command used to change file permissions. | Modifies read, write, and execute permissions for users, groups, and others. |
| Utility | umask | Command and shell setting that defines default permission mask. | Controls default permissions for newly created files and directories. |
| Utility | chown | Command used to change file ownership. | Changes the user owner of files or directories. |
| Utility | chgrp | Command used to change group ownership. | Changes the group owner of files or directories. |
| Utility | ln | Command used to create links between files. | Creates hard or symbolic links. |
| Utility | ls | Lists directory contents. | Displays file names, permissions, ownership, and other metadata. |
| Utility | find | Searches for files in a directory hierarchy. | Locates files based on name, type, permissions, size, and more. |
| Utility | locate | Searches for files using a prebuilt index database. | Quickly finds file paths. |
| Utility | updatedb | Updates the locate database. | Rebuilds the file index used by locate. |
| Utility | whereis | Locates binaries, source files, and manual pages. | Finds related program files. |
| Utility | which | Locates executable files in the PATH. | Displays the path of a command that would be executed. |
| Utility | type | Indicates how a command name would be interpreted by the shell. | Identifies whether a command is built-in, alias, function, or executable. |
| File | /etc/updatedb.conf | Configuration file for updatedb. | Defines which directories are indexed or excluded from the locate database. |

[Back](README.md)

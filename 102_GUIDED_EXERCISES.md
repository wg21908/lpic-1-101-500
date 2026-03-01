# Guided Exercises

Linux Installation and Package Management

[Back](README.md)

## Topic 102.1

| # | Question | Answer |
|---|----------|--------|
| 1 | On Linux systems, where are the files for the GRUB bootloader stored? | Under /boot/grub. |
| 2 | Where should the boot partition end to ensure that a PC will always be able to load the kernel? | Before cylinder 1024. |
| 3 | Where is the EFI partition usually mounted? | Under /boot/efi. |
| 4 | When manually mounting a filesystem, under which directory should it usually be mounted? | Under /mnt. However, this is not mandatory. You can mount a partition under any directory you want. |

[Back](README.md)

## Topic 102.2

| # | Question | Answer |
|---|----------|--------|
| 1 | What is the default location for the GRUB 2 configuration file? | /boot/grub/grub.cfg |
| 2 | What are the steps needed to change the settings for GRUB 2? | Make your changes to the file /etc/default/grub, then update the configuration with update-grub. |
| 3 | Into which file should custom GRUB 2 menu entries be added? | /etc/grub.d/40_custom |
| 4 | Where are the menu entries for GRUB Legacy stored? | /boot/grub/menu.lst |
| 5 | From a GRUB 2 or GRUB Legacy menu, how can you enter the GRUB Shell? | Press c in the menu screen. |

[Back](README.md)

## Topic 102.3

## Topic – Answers to Guided Exercises

| # | Question | Answer |
|---|----------|--------|
| 1 | Divide the following shared library names into their parts: <table><tr><th style="white-space: nowrap;">Complete file name</th></tr><tr><td style="white-space: nowrap;">linux-vdso.so.1</td></tr><tr><td style="white-space: nowrap;">libprocps.so.6</td></tr><tr><td style="white-space: nowrap;">libdl.so.2</td></tr><tr><td style="white-space: nowrap;">libc.so.6</td></tr><tr><td style="white-space: nowrap;">libsystemd.so.0</td></tr><tr><td style="white-space: nowrap;">ld-linux-x86-64.so.2</td></tr></table> | <table><tr><th style="white-space: nowrap;">Library name</th><th style="white-space: nowrap;">so suffix</th><th style="white-space: nowrap;">Version number</th></tr><tr><td style="white-space: nowrap;">linux-vdso</td><td style="white-space: nowrap;">so</td><td style="white-space: nowrap;">1</td></tr><tr><td style="white-space: nowrap;">libprocps</td><td style="white-space: nowrap;">so</td><td style="white-space: nowrap;">6</td></tr><tr><td style="white-space: nowrap;">libdl</td><td style="white-space: nowrap;">so</td><td style="white-space: nowrap;">2</td></tr><tr><td style="white-space: nowrap;">libc</td><td style="white-space: nowrap;">so</td><td style="white-space: nowrap;">6</td></tr><tr><td style="white-space: nowrap;">libsystemd</td><td style="white-space: nowrap;">so</td><td style="white-space: nowrap;">0</td></tr><tr><td style="white-space: nowrap;">ld-linux-x86-64</td><td style="white-space: nowrap;">so</td><td style="white-space: nowrap;">2</td></tr></table> |
| 2 | You have developed a piece of software and want to add a new shared library directory to your system (/opt/lib/mylib). You write its absolute path in a file called mylib.conf.<br /><br />In what directory should you put this file?<br /><br />What command should you run to make the changes fully effective? | /etc/ld.so.conf.d<br /><br />ldconfig |
| 3 | What command would you use to enumerate the shared libraries required by kill? | <nobr>ldd /bin/kill<nobr />|

[Back](README.md)

## Topic 102.4

| # | Question | Answer |
|---|----------|--------|
| 1 | What is the command to install a package named package.deb using dpkg? | Pass the -i parameter to dpkg:<br><br>`# dpkg -i package.deb` |
| 2 | Using dpkg-query, find which package contains a file named 7zr.1.gz. | Add the -S parameter to dpkg-query:<br><br>`# dpkg-query -S 7zr.1.gz` |
| 3 | Can you remove a package called unzip from the system using dpkg -r unzip if the package file-roller depends on it? If not, what would be the correct way to do it? | No. dpkg will not resolve dependencies, and will not let you remove a package if another installed package depends on it. In this example, you could first remove file-roller (assuming nothing depends on it) and then remove unzip, or remove both at the same time with:<br><br>`# dpkg -r unzip file-roller` |
| 4 | How can you find out which package contains the file /usr/bin/unrar using the apt-file utility? | Use the search parameter followed by the path (or filename):<br><br>`# apt-file search /usr/bin/unrar` |
| 5 | Using apt-cache, what is the command to show information for the package gimp? | Use the show parameter followed by the package name:<br><br>`# apt-cache show gimp` |

[Back](README.md)

## Topic 102.5

| # | Question | Answer |
|---|----------|--------|
| 1 | Using rpm on a Red Hat Enterprise Linux system, how would you install the package file-roller-3.28.1-2.el7.x86_64.rpm showing a progress bar during the installation? | Use the -i parameter to install a package, and the -h option to enable “hash marks” showing installation progress. So, the answer is: `rpm -ih file-roller-3.28.1-2.el7.x86_64.rpm`. |
| 2 | Using rpm, find out which package contains the file /etc/redhat-release. | You are querying information about a file, so use the -qf parameter: `rpm -qf /etc/redhat-release`. |
| 3 | How would you use yum to check for updates for all packages in the system? | Use the check-update operation without a package name: `yum check-update`. |
| 4 | Using zypper, how would you disable a repository called repo-extras? | Use the modifyrepo operation to change the parameters of a repo, and the -d parameter to disable it: `zypper modifyrepo -d repo-extras`. |
| 5 | If you have a .repo file describing a new repository, where this file should be put so that it is recognized by DNF? | .repo files for DNF should be put on the same place used by YUM, inside `/etc/yum.repos.d/`. |

[Back](README.md)

## Topic 102.6

| # | Question | Answer |
|---|----------|--------|
| 1 | What CPU extensions are necessary on an x86 based hardware platform that will run fully virtualized guests? | VT-x for Intel CPUs or AMD-V for AMD CPUs |
| 2 | A mission-critical server installation that will require the fastest performance will likely use what type of virtualization? | An operating system that makes use of paravirtualization, such as Xen, as the guest operating system can make better use of hardware resources available to it through the use of software drivers designed to work with the hypervisor. |
| 3 | Two virtual machines that have been cloned from the same template and that utilize D-Bus are performing erratically. They both have separate hostnames and network configuration settings. What command would be used to determine if each of the virtual machines have different D-Bus Machine IDs? | `dbus-uuidgen --get` |

[Back](README.md)
  

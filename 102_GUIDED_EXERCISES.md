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

[Back](README.md)

## Topic 102.5

[Back](README.md)

## Topic 102.6

[Back](README.md)
  

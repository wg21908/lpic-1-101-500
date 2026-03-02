# Guided Exercises

GNU and Unix Commands

[Back](README.md)

## Topic 103.1

| # | Question                                                                                                                                    | Answer                                                                                                                                             |
| - | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 | Use the man system to determine how to tell apropos to output a brief command so that it outputs only a brief usage message and then exits. | Run man apropos and scroll down through the “Options” section until you get to the --usage paragraph.                                              |
| 2 | Use the man system to determine which copyright license is assigned to the grep command.                                                    | Run man grep and scroll down to the “Copyright” section of the document. Note that the program uses a copyright from the Free Software Foundation. |
| 3 | Use the export command to add a new directory to your path (this will not survive a reboot). You can temporarily add a new directory (perhaps one called myfiles that lives in your home directory) to your path using export PATH="/home/yourname/myfiles:$PATH". Create a simple script in the myfiles/ directory, make it executable, and try to run it from a different directory. These commands assume you’re in your home directory which contains a directory called myfiles. $ touch myfiles/myscript.sh $ echo '#!/bin/bash' >> myfiles/myscript.sh $ echo 'echo Hello' >> myfiles/myscript.sh $ chmod +x myfiles/myscript.sh $ myscript.sh Hello | You can temporarily add a new directory (perhaps one called myfiles that lives in your home directory) to your path using export PATH="/home/yourname/myfiles:$PATH". Create a simple script in the myfiles/ directory, make it executable, and try to run it from a different directory. These commands assume you’re in your home directory which contains a directory called myfiles. $ touch myfiles/myscript.sh $ echo '#!/bin/bash' >> myfiles/myscript.sh $ echo 'echo Hello' >> myfiles/myscript.sh $ chmod +x myfiles/myscript.sh $ myscript.sh Hello |
| 4 | Use the unset command to delete the PATH variable. Try running a command (like sudo cat /etc/shadow) using sudo. What happened? Why? (Exiting your shell will return you to your original state.)                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Typing unset PATH will erase the current path settings. Trying to invoke a binary without its absolute address will fail. For that reason, trying to run a command using sudo (which itself is a binary program located in /usr/bin/sudo) will fail — unless you specify the absolute location, as in: /usr/bin/sudo /bin/cat /etc/shadow. You can reset your PATH using export or by simply exiting from the shell.                                                                                                                                           |


[Back](README.md)

## Topic 103.2

| # | Question                                                                                                                                    | Answer                                                                                                                                             |
| - | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 | | |
| 2 | | |
| 3 | Consider this /etc/passwd file example. Copy the lines below to a local file named mypasswd for this exercise. | <table><th></th><tr><td>root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
nvidia-persistenced:x:121:128:NVIDIA Persistence Daemon,,,:/nonexistent:/sbin/nologin
libvirt-qemu:x:64055:130:Libvirt Qemu,,,:/var/lib/libvirt:/usr/sbin/nologin
libvirt-dnsmasq:x:122:133:Libvirt Dnsmasq,,,:/var/lib/libvirt/dnsmasq:/usr/sbin/nologin
carol:x:1000:2000:Carol Smith,Finance,,,Main Office:/home/carol:/bin/bash
dave:x:1001:1000:Dave Edwards,Finance,,,Main Office:/home/dave:/bin/ksh
emma:x:1002:1000:Emma Jones,Finance,,,Main Office:/home/emma:/bin/bash
frank:x:1003:1000:Frank Cassidy,Finance,,,Main Office:/home/frank:/bin/bash
grace:x:1004:1000:Grace Kearns,Engineering,,,Main Office:/home/grace:/bin/ksh
henry:x:1005:1000:Henry Adams,Sales,,,Main Office:/home/henry:/bin/bash
john:x:1006:1000:John Chapel,Sales,,,Main Office:/home/john:/bin/bash</td></tr></table> |

[Back](README.md)

## Topic 103.3


[Back](README.md)

## Topic 103.4


[Back](README.md)

## Topic 103.5


[Back](README.md)

## Topic 103.6


[Back](README.md)

## Topic 103.7

| # | Question                                                                                                                                   | Answer                                              |
| - | ------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------- | 
| 1 | What extended regular expression would match any email address, like [info@example.org](mailto:info@example.org)?                          | egrep "\S+@\S+.\S+"                                 | 
| 2 | What extended regular expression would only match any IPv4 address in the standard dotted-quad format, like 192.168.15.1?                  | egrep "[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}" | 
| 3 | How can the grep command be used to list the contents of file /etc/services, discarding all comments (lines starting with #)?              | grep -v ^# /etc/services                            |
| 4 | The file domains.txt contains a list of domain names, one per line. How would the egrep command be used to list only .org or .com domains? | egrep ".org$\| .com$" domains.txt |
| 5 | Command last shows a listing of last logged in users, including their origin IPs. How would the egrep command be used to filter last output, showing only occurrences of an IPv4 address, discarding any additional information in the corresponding line? | last -i \| egrep -o '[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}' |
| 6 | What option should be given to grep in order to correctly filter the output generated by command find executed with option -print0?   | The option -z or --null-data, as in find . -print0 \| grep -z expression. |
| 7 | Command uptime -s shows the last date when the system was powered on, as in 2019-08-05 20:13:22. What will be the result of command uptime -s \| sed -e 's/(.*) (.*)/\1/'?  | An error will occur. By default, parenthesis should be escaped to use backreferences in sed. |
| 8 | What option should be given to grep so it counts matching lines instead of displaying them?   | Option -c.  |

[Back](README.md)

## Topic 103.8

| # | Question                                                                                                                                                                                                                                                                                                              | Answer                                                                                                                                         |
| - | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 | vi is most used as an editor for configuration files and source code, where indentation helps to identify sections of text. A selection can be indented to the left by pressing < and to the right by pressing >. What keys should be pressed in normal mode to indent the current selection three steps to the left? | The keys 3<, meaning three steps to the left.                                                                                                  |
| 2 | An entire line can be selected by pressing V in vi normal mode. However, the terminating newline character is also included. What keys should be pressed in normal mode to select from the starting character until, but not including, the newline character?                                                        | The keys 0v$h, meaning 0 (“jump to start of a line”), v (“start character selection”), $ (“go to end of line”) and h (“go back one position”). |
| 3 | How should vi be executed in the command line to open ~/.bash_profile and jump straight to the last line?                                                                                                                                                                                                             | The command vi + ~/.bash_profile will open the file and place the cursor at its last line.                                                     |
| 4 | What keys should be pressed in vi normal mode to delete characters from the current cursor position until the next period character?                                                                                                                                                                                  | The keys dt., meaning d (“start deletion”), t (“jump to the following character”) and . (period character).                                    |


[Back](README.md)

# Files, Terms & Utilities

GNU and Unix Commands

[Back](README.md)

## Topic 103

| Category | Item | Definition | Purpose |
|----------|------|------------|----------|
| Utility | bash | Bourne Again SHell; a command-line interpreter and scripting shell. | Executes commands, runs scripts, and provides the user interface to the system shell. |
| Utility | echo | Command that prints arguments to standard output. | Displays text or variable values in the terminal or scripts. |
| Utility | env | Command that displays or runs a program in a modified environment. | Used to view environment variables or run commands with specific environment settings. |
| Built-in | export | Shell built-in command that marks variables to be exported to child processes. | Makes shell variables available to subshells and executed programs. |
| Utility | pwd | Print Working Directory command. | Displays the current directory path. |
| Built-in | set | Shell built-in that sets shell options or positional parameters. | Configures shell behavior and displays shell variables and functions. |
| Built-in | unset | Shell built-in that removes variable or function definitions. | Deletes environment or shell variables. |
| Utility | type | Command that indicates how a command name would be interpreted by the shell. | Identifies whether a command is a built-in, alias, function, or executable file. |
| Utility | which | Command that locates a command’s executable file in the PATH. | Displays the filesystem path of a command. |
| Utility | man | Manual page viewer. | Displays documentation for commands and topics. |
| Utility | uname | Prints system information. | Shows kernel name, version, architecture. |
| Utility | history | Displays previously executed commands. | Review and reuse past commands. |
| File | .bash_history | File storing Bash command history. | Persists command history between sessions. |
| Term | Quoting | Mechanism to preserve literal meaning of characters in shell. | Controls variable expansion and interpretation. |
| Utility | cat | Concatenates and displays file contents. | View or combine files. |
| Utility | head | Displays first lines of a file. | Preview beginning of files. |
| Utility | tail | Displays last lines of a file. | Monitor logs or file endings. |
| Utility | less | Pager program for viewing files. | Scroll through file contents interactively. |
| Utility | cut | Extracts sections from lines of input. | Select specific columns or fields. |
| Utility | paste | Merges lines of files. | Combine files column-wise. |
| Utility | nl | Numbers lines of files. | Display file with line numbers. |
| Utility | od | Dumps file contents in octal/hex format. | Inspect binary file content. |
| Utility | wc | Counts lines, words, bytes. | File statistics. |
| Utility | sort | Sorts lines of text. | Organize output alphabetically or numerically. |
| Utility | uniq | Filters duplicate adjacent lines. | Remove duplicate entries. |
| Utility | tr | Translates or deletes characters. | Character substitution. |
| Utility | split | Splits files into pieces. | Divide large files. |
| Utility | sed | Stream editor. | Perform text transformations. |
| Utility | grep | Searches text using patterns. | Pattern matching in files. |
| Utility | egrep | Extended grep (uses extended regex). | Advanced pattern matching. |
| Utility | fgrep | Fixed-string grep. | Literal string matching. |
| Term | regex(7) | Regular expression syntax specification. | Defines pattern matching rules. |
| Utility | md5sum | Calculates MD5 checksum. | Verify file integrity. |
| Utility | sha256sum | Calculates SHA-256 checksum. | Stronger integrity verification. |
| Utility | sha512sum | Calculates SHA-512 checksum. | Strong integrity verification. |
| Utility | gzip | Compresses files using gzip. | Reduce file size. |
| Utility | gunzip | Decompresses gzip files. | Extract compressed files. |
| Utility | bzip2 | Compresses files using bzip2. | Higher compression ratio. |
| Utility | bunzip2 | Decompresses bzip2 files. | Extract bzip2 archives. |
| Utility | zcat | Displays compressed file contents. | View gzip file without decompressing. |
| Utility | bzcat | Displays bzip2 compressed contents. | View bzip2 file without decompressing. |
| Utility | xzcat | Displays xz compressed contents. | View xz file without decompressing. |
| Utility | tar | Archive utility. | Create/extract archive files. |
| Utility | cpio | Archive utility. | Copy files to/from archives. |
| Utility | dd | Low-level data copying tool. | Disk imaging and raw data copying. |
| Utility | file | Determines file type. | Identify file format. |
| Utility | cp | Copies files/directories. | Duplicate files. |
| Utility | mv | Moves/renames files. | Relocate or rename files. |
| Utility | rm | Removes files. | Delete files. |
| Utility | rmdir | Removes empty directories. | Delete directories. |
| Utility | mkdir | Creates directories. | Make new directories. |
| Utility | ls | Lists directory contents. | View files. |
| Utility | touch | Creates empty file or updates timestamp. | File creation or timestamp modification. |
| Utility | find | Searches for files in directory tree. | Locate files by criteria. |
| Term | file globbing | Shell pattern matching using wildcards (*, ?, []). | Match filenames in shell. |
| Utility | tee | Reads input and writes to file and stdout. | Save and display output simultaneously. |
| Utility | xargs | Builds argument list from stdin. | Pass input as command arguments. |
| Operator | & | Runs command in background. | Execute asynchronously. |
| Utility | bg | Resumes stopped job in background. | Background job control. |
| Utility | fg | Brings job to foreground. | Foreground job control. |
| Utility | jobs | Lists active jobs. | View job status. |
| Utility | kill | Sends signal to process. | Terminate or signal processes. |
| Utility | killall | Sends signal to processes by name. | Kill processes by name. |
| Utility | pgrep | Searches processes by name. | Find process IDs. |
| Utility | pkill | Sends signal to processes by name. | Kill matching processes. |
| Utility | ps | Displays process status. | View running processes. |
| Utility | top | Real-time process monitor. | Monitor system performance. |
| Utility | free | Displays memory usage. | View RAM and swap usage. |
| Utility | uptime | Shows system uptime. | Check system load and running time. |
| Utility | watch | Executes program repeatedly. | Monitor changing output. |
| Utility | nice | Runs command with modified priority. | Set CPU scheduling priority. |
| Utility | renice | Changes priority of running process. | Adjust process priority. |
| Utility | nohup | Runs command immune to hangups. | Keep process running after logout. |
| Utility | screen | Terminal multiplexer. | Manage multiple terminal sessions. |
| Utility | tmux | Terminal multiplexer. | Advanced session management. |
| Editor | vi | Modal text editor. | Edit text files. |
| vi Command | /, ? | Search forward/backward in vi. | Navigate via search. |
| vi Command | h, j, k, l | Cursor movement keys in vi. | Navigate text. |
| vi Command | i, o, a | Insert mode commands in vi. | Enter insert mode. |
| vi Command | d, p, y, dd, yy | Delete, paste, yank commands. | Edit text. |
| vi Command | ZZ, :w!, :q! | Save/quit commands. | Exit and save control. |
| Variable | EDITOR | Environment variable specifying default editor. | Defines editor used by system utilities. |

[Back](README.md)

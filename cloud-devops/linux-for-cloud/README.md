# Linux for Cloud & DevOps Engineers

Linux is based on UNIX and hence it borrows its filesystem hierarchy from UNIX.

![Linux directory structure2](./assets/linux-system-directoies-poster.png)

## How to SSH using Linux

### AWS: EC2 Instance connect
`ssh -i "FileName.pem" ec2-user@ec2-IP.compute-1.amazonaws.com`

In case of error

`@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@

@         WARNING: UNPROTECTED PRIVATE KEY FILE!          @

@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@`

run chmod 0400 command

`chmod 0400 FileName.pem`


## Bash Commands
| Syntax | Description |
| ----------- | ----------- |
| uname -a | Show system and kernel |
| head -n1 /etc/issue | Show distri­bution |
| mount | Show mounted filesy­stems |
| date | Show system date |
| uptime | Show uptime |
| whoami | Show your username |

## Bash Variables
| Syntax | Description |
| ----------- | ----------- |
| env |Show enviro­nment variables |
| echo $NAME | Output value of $NAME variable |
| export NAME=value | Set $NAME to value |
| $PATH | Executable search path |
| $HOME | Home directory |
| $SHELL | Current shell |

## IO Redire­ction
| Syntax | Description |
| ----------- | ----------- |
| cmd < file | Input of cmd from file|
| cmd1 <(cmd2) | Output of cmd2 as file input to cmd1 |
| cmd > file | Standard output (stdout) of cmd to file |
| cmd > /dev/null |Discard stdout of cmd |
| cmd >> file | Append stdout to file |
| cmd 2> file | Error output (stderr) of cmd to file |
| cmd 1>&2 | stdout to same place as stderr |
| cmd 2>&1 | stderr to same place as stdout |
| cmd &> file | Every output of cmd to file |

## Pipes
| Syntax | Description |
| ----------- | ----------- |
| cmd1 | cmd2 | stdout of cmd1 to cmd2  
| cmd1 |& cmd2| stderr of cmd1 to cmd2


## Files and Directories

### Directory Operations
| Syntax | Description |
| ----------- | ----------- |
| pwd | Show current directory
| mkdir *dir* |Make directory dir |
| rmdir *dir* |Remove  directory dir |
| cd *dir* | Change directory to dir |
| cd *..* | Go up a directory |
| ls *<option>* | list files | 

| ls <option> | Description |
| ----------- | ----------- |
| ls -a | Show all (including hidden) |
| ls -R | Recursive list |
| ls -r | Reverse order |
| ls -t | Sort by last modified |
| ls -S | Sort by file size |
| ls -l | Long listing format |
| ls -1 | One file per line |
| ls -m | Comma-­sep­arated output |

## File Operations
| Syntax | Description |
| ----------- | ----------- |
| touch *file1* | Create file1 |
| cat *file1 file2* | Concat­enate files and output|
| less *file1* | View and paginate file1 |  
| file *file1* | Get type of file1|
| cp *file1 file2* | Copy file1 to file2|
| mv file1 file2 | Move file1 to file2 |
| rm file1 | Delete file1 |
| head file1 | Show first 10 lines of file1|
| tail file1 | Show last 10 lines of file1|
| tail -F file1 | Output last lines of file1 as it changes|

## Search Operations
| Syntax | Description |
| ----------- | ----------- |
| find *dir* *-option* | find a file, it will look for in *-dir*. Options: [-name, -user, -group]|
| find . -name *file* | find a file, it will look for in current and sub-directories |
| sudo find / -name *file* | find a file, it will look for in all directories |
| find */home/username/* -name *"*jpg"* -mtime *4* | find a file, it will look for in /home/randomuser/ and have been modified in the preceding 4 days  |
| whereis command | Find binary / source / manual for command|
| locate file | Find file (quick search of system index) |


## Find files bases on content 

| Syntax | Description |
| ----------- | ----------- |
| diff [OPTION]... FILES | Compare FILES line by line.|
| diff *file1* *file* | Compare FILES (file1 and file2) line by line.|

| Syntax | Description |
| ----------- | ----------- |
| grep [OPTION...] PATTERNS [FILE...] | searches  for  PATTERNS  in  each  FILE.|
| grep hol file* | search "hol" in "file*" | search "hol" in "file*" |

`file1:hole

file2:hola

file2:hola2
`
| Syntax | Description |
| ----------- | ----------- |
| sed [OPTION]... {script-only-if-no-other-script} [input-file]... | sA stream editor is used to perform basic text transformations on an input
       stream (a file or input from a pipeline)|
| sed *'s/old_text/new_text/'* *filename* | replace old_text by new_text in file_name |
| sed *'s/old_text/new_text/g'* *filename* | replace old_text by new_text in file_name global |

## User Management


## Networking


## Services


## Process Management


## Other Topics











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

## User Management


## Networking


## Services


## Process Management


## Other Topics











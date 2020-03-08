 ![Linux](img/linux.jpg)

##Table of contents

- [Linux Commands](#linux-commands)
  - [Managing files/directories](#managing-files-/-directories)
  - [File system management](#file-system-management)
  - [Process management](#process-management)
  - [Managing users, groups and the system](#managing-users-,-groups-and-the-system)
  - [I/O commands](#i/o-commands)
  - [Network](#network)
  - [Hardware support](#hardware-support)
  - [Other](#other)

# Linux commands

## Managing files/directories
- `cd examlpe` -- change directory to example
  - `cd ..` -- move up one directory 
  - `cd ../..` -- move up two directory 
  - `cd ~` -- change to home directory
- `pwd` -- shows the name of the working directory
- `mkdir directory_name` -- create new directory
- `rmdir directory_name` -- remove empty directory
- `rm {options} name` -- remove file (by default it does not remove directories)
  - Options (most popular)
    - f - ignore non-existing files  
    - r - remove directories and their contents
    - i - prompt before every removal
    - v - explain at all time what is being done
- `ls {options}` -- lists information about files and directories.
  - Options (most popular)
    - t - sort the file by modification time
    - 1 - display one file per line 
    - l - display all information about files/directories
    - a - do not ignore hidden files
- `mv {options} source destination` -- moves and renames files and directories.
  - `mv {options} file_name1 file_name2` - rename file named file_name1 to file_name2
  - `mv {options} file_name [file_name2...] destination` - move source file(s) to destination
  - Options (most popular)
    - i - prompt before overwriting an existing file
    - n - never overwrite an existing file
- `cp {options} from to`  -- copy files or directories
  - Options (most popular):
    - i - ask for permission before user overwrite the destination file
    - r - copy the entire directory structure.
    - p - preserves the the time of the last data modification and the time of the last access, the ownership 
    and the file permission-bits of each source file in the corresponding destination
    file. 
- `touch file_name`  -- create empty file
- `wc file_name` -- show information about the file: number of lines, word count, byte and characters count 
- `cat {options} file_name` -- reads data from the file and gives their content as output
  - `cat >file_name` - create new file with content
  - `cat >>file_name` - append content to the end of file_name
  - `cat file1 >> file2` - append the contents of file1 to the end of file2
  - Options (most popular):
    - n - number all output lines
    - b - number non-empty output lines
- `tail {options} file_name` -- output the last part of files.
  - Options (most popular):
    - n nums - print the last nums lines, instead of the default 10.
    - f - output appended data as the file grows 
- `head {options} file_name` -- output the first part of files.
  - Options (most popular):
    - n nums - print the first nums lines, instead of the default 10.
- `less file_name` -- display file contents one page at the time
  - Key commands (most popular):
    - space bar - move down one page
    - b - move up one page
    - g - go to the first line  
    - /search_term - search forward from the current position for the search_term string
    - ?search_term - search backward from the current position for the search_term string
    - n - when searching, to to the next occurrence
    - N - when searching, go to the previous occurrence
- `gedit` -- text editor for the GNOME Desktop
- `chmod`




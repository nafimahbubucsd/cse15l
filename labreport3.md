 LABREPORT3 : NAFI MAHBUB
 
 
 I'll pick the `grep` command for this task, which is a command-line utility for searching plain-text data sets for lines that match a regular expression. It's very useful when looking for specific patterns in files.


1. `-i` option: This option makes `grep` ignore case distinctions in both the pattern and the input files. 

Example 1:
```
$ grep -i 'error' ./technical/logfile.txt
```
This command searches for the term 'error' in `logfile.txt` file located in the `./technical` directory, disregarding case.

Example 2:
```
$ grep -i 'function' ./technical/*.c
```
This command searches for the term 'function' in all `.c` files in the `./technical` directory, ignoring case. This is useful when searching in languages where keywords are case insensitive.

2. `-r` or `-R` option: This option makes `grep` search for a string in files and directories recursively.

Example 1:
```
$ grep -r 'main' ./technical/
```
This command searches for the string 'main' in all files under the `./technical` directory recursively. 

Example 2:
```
$ grep -R 'ERROR' ./technical/
```
This command will recursively search for the string 'ERROR' in all files under the `./technical` directory.

3. `-v` option: This option inverts the sense of matching, to select non-matching lines.

Example 1:
```
$ grep -v 'error' ./technical/logfile.txt
```
This command outputs all lines from `logfile.txt` that do not contain the term 'error'.

Example 2:
```
$ grep -v 'success' ./technical/logfile.txt
```
This command outputs all lines from `logfile.txt` that do not contain the term 'success'. This is useful when you're interested in lines that do not contain certain patterns.

4. `-l` option: This option makes `grep` print only names of files containing the match.

Example 1:
```
$ grep -l 'main' ./technical/*
```
This command will output names of all files under the `./technical` directory that contain the term 'main'.

Example 2:
```
$ grep -l 'error' ./technical/*
```
This command will output names of all files under the `./technical` directory that contain the term 'error'. This is useful when you just want to know which files contain the pattern, not the actual matching lines.

Sources: 
- https://man7.org/linux/man-pages/man1/grep.1.html
- https://www.geeksforgeeks.org/grep-command-in-unixlinux/
- ChatGPT

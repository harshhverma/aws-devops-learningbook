## Linux Basic Commands (AWS EC2 Practice)

## Environment
- AWS EC2 (ubuntu)
- Connected using MobaXterm
- Practicing basic Linux & shell commands

---

## 1 ls – List Directory Contents

Used to display files and directories in the current directory.

### Basic Usage

Common Options
ls -l     # Long listing format
ls -a     # Show hidden files
ls -la    # Long format + hidden files
## 2 touch – Create Empty File

Creates a new empty file.

touch filename.txt

Example:

touch script.sh
## 3 cat – Display File Content

Used to view file content.

cat filename.txt

Example:

cat script.sh

## 4 vim – Text Editor

Used to create and edit files inside Linux.

vim filename.txt
Basic Vim Commands

i → Insert mode

Esc → Exit insert mode

:w → Save

:q → Quit

:wq → Save & Quit

## 5 chmod – Change File Permissions

Used to modify file permissions.

chmod 755 filename.sh
Permission Numbers
Number	Permission
7	Read + Write + Execute
6	Read + Write
5	Read + Execute
4	Read only

## Example:

chmod +x script.sh

Makes the script executable.

## 6 man – Manual Page

Used to read documentation for commands.

man ls

Press q to exit manual page.

## Learning Outcome

Understood basic Linux commands

Practiced file creation and editing

Learned permission management

Built foundation for Shell Scripting & DevOps

## Goal

Building strong Linux fundamentals for Cloud / DevOps / SRE roles.

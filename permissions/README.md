# Permissions Project - Holberton School

## Introduction

## Task List

1. *My name is Betty*
   - Switches the current user to betty.

2. *Who am I*
   - Prints the effective username of the current user.

3. *Groups*
   - Prints all the groups the current user is part of.

4. *New Owner*
   - Changes the owner of the file hello to betty.

5. *Empty!*
   - Creates an empty file named hello.

6. *Execute*
   - Adds execute permission to the owner of the file hello.

7. *Multiple Permissions*
   - Adds execute permission to the owner and the group owner, and read permission to other users for the file hello.

8. *Everybody!*
   - Adds execute permission to the owner, group owner, and other users for the file hello.

9. *James Bond*
   - Sets the file hello permissions as follows:
     - No permissions for the owner
     - No permissions for the group
     - All permissions for other users

10. *John Doe*
    - Sets the file hello permissions to 753.

11. *Look in the mirror*
    - Sets the mode of hello to be the same as olleh.

12. *Directories*
    - Adds execute permission to all subdirectories in the current directory for the owner, the group, and all other users. Regular files should not be changed.

13. *More directories*
    - Creates a directory named my_dir with permissions 751.

14. *Change group*
    - Changes the group owner of the file hello to school.

15. *Change owner and group*
    - Changes the owner to vincent and the group to staff for all files and directories in the working directory.

16. *Symbolic Links*
    - Changes the owner and the group owner of the symbolic link hello to vincent and staff, respectively.

17. *If Only*
    - Changes the owner of the file hello to vincent only if it is currently owned by guillaume.

## How to Run the Scripts

1. Make sure the script is executable:
   bash
   chmod +x script_name
   
2. Execute the script:
   bash
   ./script_name
   
3. Verify the changes:
   bash
   ls -l filename
   

## Project Requirements

- Use only vi, vim, emacs editors.
- All scripts must run on Ubuntu 22.04 LTS.
- Each script must be exactly two lines long.
- All files must end with a new line.
- The first line of all scripts must be #!/bin/bash.
- Not allowed to use: &&, ||, or ;.
- All files must be executable.


This script changes the owner of the file hello
Permissions Project - Holberton School

Introduction

This project teaches me how to manage file and directory permissions in Linux. Each script in this project performs a specific task to modify or adjust permissions.

Task List

0. My name is Betty

🔹 Description:
Switches the current user to betty.

🔹 Command:

#!/bin/bash
exec su betty

1. Who am I

🔹 Description:
Prints the effective username of the current user.

🔹 Command:

#!/bin/bash
exec whoami

2. Groups

🔹 Description:
Prints all the groups the current user is part of.

🔹 Command:

#!/bin/bash
exec groups

3. New Owner

🔹 Description:
Changes the owner of the file hello to betty.

🔹 Command:

#!/bin/bash
exec chown betty hello

4. Empty!

🔹 Description:
Creates an empty file named hello.

🔹 Command:

#!/bin/bash
exec touch hello

5. Execute

🔹 Description:
Adds execute permission to the owner of the file hello.

🔹 Command:

#!/bin/bash
exec chmod u+x hello

6. Multiple Permissions

🔹 Description:
Adds execute permission to the owner and the group owner, and read permission to other users for the file hello.

🔹 Command:

#!/bin/bash
exec chmod ug+x,o+r hello

7. Everybody!

🔹 Description:
Adds execute permission to the owner, group owner, and other users for the file hello.

🔹 Command:

#!/bin/bash
exec chmod a+x hello

8. James Bond

🔹 Description:
Sets the file hello permissions as follows:
    •   No permissions for the owner
    •   No permissions for the group
    •   All permissions for other users

🔹 Command:

#!/bin/bash
exec chmod 007 hello

9. John Doe

🔹 Description:
Sets the file hello permissions to 753.

🔹 Command:

#!/bin/bash
exec chmod 753 hello

10. Look in the mirror

🔹 Description:
Sets the mode of hello to be the same as olleh.

🔹 Command:

#!/bin/bash
exec chmod --reference=olleh hello

11. Directories

🔹 Description:
Adds execute permission to all subdirectories in the current directory for the owner, the group, and all other users. Regular files should not be changed.

🔹 Command:

#!/bin/bash
exec find . -type d -exec chmod a+x {} \;

12. More directories

🔹 Description:
Creates a directory named my_dir with permissions 751.

🔹 Command:

#!/bin/bash
exec mkdir -m 751 my_dir

13. Change group

🔹 Description:
Changes the group owner of the file hello to school.

🔹 Command:

#!/bin/bash
exec chgrp school hello

14. Change owner and group

🔹 Description:
Changes the owner to vincent and the group to staff for all files and directories in the working directory.

🔹 Command:

#!/bin/bash
exec chown -R vincent:staff .

15. Symbolic Links

🔹 Description:
Changes the owner and the group owner of the symbolic link hello to vincent and staff, respectively.

🔹 Command:

#!/bin/bash
exec chown -h vincent:staff hello.

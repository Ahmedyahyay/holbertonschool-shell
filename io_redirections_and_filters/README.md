0-hello_world
    •   Prints "Hello, World" followed by a new line to the standard output.
    •   Command used: echo

1-confused_smiley
    •   Displays a confused smiley face: "(Ôo)'
    •   Command used: echo

2-hellofile
    •   Displays the content of the /etc/passwd file.
    •   Command used: cat /etc/passwd

3-twofiles
    •   Displays the content of /etc/passwd and /etc/hosts.
    •   Command used: cat /etc/passwd /etc/hosts

4-lastlines
    •   Displays the last 10 lines of the /etc/passwd file.
    •   Command used: tail -n 10 /etc/passwd

5-firstlines
    •   Displays the first 10 lines of the /etc/passwd file.
    •   Command used: head -n 10 /etc/passwd

6-third_line
    •   Displays the third line of the file iacta.
    •   Command used: sed -n '3p' iacta

7-file
    •   Creates a file named \\\'"Best School"\'\\$\?\\\\\*:) containing the text "Best School" followed by a new line.
    •   Command used: echo "Best School" > '\\\'"Best School"\'\\$\?\\\\\*:)'

8-cwd_state
    •   Saves the result of ls -la into the file ls_cwd_content, overwriting if it exists.
    •   Command used: ls -la > ls_cwd_content

9-duplicate_last_line
    •   Duplicates the last line of the file iacta.
    •   Command used: tail -n 1 iacta >> iacta

10-no_more_js
    •   Deletes all .js files in the current directory and subdirectories.
    •   Command used: find . -type f -name "*.js" -delete

11-directories
    •   Counts the number of directories and subdirectories in the current directory (excluding . and ..).
    •   Command used: find . -type d | wc -l

12-newest_files
    •   Displays the 10 newest files in the current directory, sorted from newest to oldest.
    •   Command used: ls -lt | head -n 10

13-unique
    •   Prints only words that appear exactly once from a list of words.
    •   Command used: sort | uniq -u

14-findthatword
    •   Displays lines containing the word "root" from the /etc/passwd file.
    •   Command used: grep "root" /etc/passwd

15-countthatword
    •   Counts the number of lines that contain the word "bin" in /etc/passwd.
    •   Command used: grep -c "bin" /etc/passwd

16-whatsnext
    •   Displays lines containing "root" and the 3 lines after each occurrence in /etc/passwd.
    •   Command used: grep -A 3 "root" /etc/passwd

17-hidethisword
    •   Displays all lines in /etc/passwd that do not contain "bin".
    •   Command used: grep -v "bin" /etc/passwd

18-letteronly
    •   Displays only lines that start with a letter from /etc/ssh/sshd_config.
    •   Command used: grep "^[a-zA-Z]" /etc/ssh/sshd_config

19-AZ
    •   Replaces all occurrences of A with Z and c with e in the input.
    •   Command used: tr 'Ac' 'Ze'

20-hiago
    •   Removes all occurrences of c and C from the input.
    •   Command used: tr -d 'cC'

21-reverse
    •   Reverses the input text.
    •   Command used: rev

22-users_and_homes
    •   Displays all users and their home directories from /etc/passwd, sorted by username.

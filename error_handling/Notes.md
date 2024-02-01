## Notes
- All succesful commands for status codes are 0, anything else is an error code, you can define these error codes inside scripts
```bash
#!/bin/bash

expr 1 + 5
echo $?

rm doodles.sh
echo $?

expr 10 + 10
echo $?
```

Outputs
```bash
[root@bb40367f0b1c bin]# exitcodes.sh
6
0
rm: cannot remove 'doodles.sh': No such file or directory
1
20
0
```
Below we can tell the shell to exit the moment it gets an error
```bash
#!/bin/bash
set -e #This tells the shell that the moment it receives an error, itll dump out of the shell
expr 1 + 5
echo $?

rm doodles.sh
echo $?

expr 10 + 10
echo $?
```
Output
```bash
[root@bb40367f0b1c bin]# exitcodes.sh
6
0
rm: cannot remove 'doodles.sh': No such file or directory
```
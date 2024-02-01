## Notes

Bash scripts only set environments within the bash session that is running in the script

Check out belows script that wont apply the environment variables to anything outside the sub shell

```bash
#!/bin/bash

MYUSERNAME="username"
MYPASSWORD="password123"
STARTOFSCRIPT=`date`

echo "My login name for this application is: $MYUSERNAME"
echo "My login password for this application is: $MYPASSWORD"
echo "This script started at: $STARTOFSCRIPT"

ENDOFSCRIPT=`date`

echo "The script ended at: $ENDOFSCRIPT"
```
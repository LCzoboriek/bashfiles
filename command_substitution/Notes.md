## Notes

```bash
#!/bin/bash
# This script is intended to show how to do simple substitution
shopt -s expand_aliases # This turns on running alias's within a subshell
alias TODAY="date" # We do double quotes here as its an alias command, its not like below with running the command, this wont run the date command but assign TODAY to run date
alias UFILES="find /home -user $USER"

TODAYSDATE=`date` #Anything within backtics will be ran as a command within a script
USERFILES=`find /home -user user` # This will find all the files in the home directory, owned by the user, called user
echo "Todays date: $TODAYSDATE"
echo "All files owned by $USER: $USERFILES"

A=`TODAY`
B=`UFILES`
echo "With Alias, TODAY is: $A"
echo "With Alias, UFILES is: $B"
```



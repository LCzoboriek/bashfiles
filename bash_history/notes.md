## Notes

- Bash history is a history of what the user has typed in the shell session
- By default the history configuration is an ENV variable. And typically its the last 100 commands, but you can control that with the HISTCONTROL var

  ```bash
  [root@localhost ~]# env | grep HISTCONTROL
  HISTCONTROL=ignoredups
  ```

- You can control the env and to make sure a command is not captured in the bash history. The ignorespace directive does exactly this

  ```bash
  [root@localhost ~]# export HISTCONTROL=$HISTCONTROL:ignorespace
  [root@localhost ~]# env | grep HISTCONTROL
  HISTCONTROL=ignoredups:ignorespace

  ```

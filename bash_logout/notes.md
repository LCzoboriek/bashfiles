## Notes

- Something thats typically not used very often is the bash_logout script.
- By default, this does nothing. This is ran when you run the `exit` command
- It gives you the ability to always do something when you exit the terminal session
- Lets say you want to wipe any potentially set envs for a shared user.
  ```
  # ~/.bash_logout
  cp ~/.bashrc.original ~/.bashrc
  ```

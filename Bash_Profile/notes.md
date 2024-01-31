## Notes

- Bash_profiles are denoted with a period at first due to the fact that they are specific for that particular user
- Typically in a bash_profile the first thing that is run is .bashrc like below

  ```

  # .bash_profile

  # Get the aliases and functions

  if [ -f ~/.bashrc ]; then
  . ~/.bashrc
  fi

  # User specific environment and startup programs

  PATH=$PATH:$HOME/bin # You then can add stuff like this, where itll append anything in the bin folder to the running environment for the current path for that user

  export PATH # This then applies the path to the running session

  alias lZ='ls -alZ | more' # You can also add alias's that you want in that particular session
  ```

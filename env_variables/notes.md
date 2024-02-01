## Notes


```bash
#!/bin/bash

clear

echo "This script will give us environment information"
echo "================================================"
echo ""
echo "Hello Username: $USER"
echo ""
echo "Your home dir is: $HOME"
echo ""
echo "Your History File Will Ignore: $HISTCONTROL"
echo ""
echo "Your Terminal Session Type is: $TERM"
echo ""
```

The above is a way to echo out your environment variables, with the user, home dir, histcontrol and the terminal session. In this case the output was

```bash
This script will give us environment information
================================================

Hello Username: cloud_user

Your home dir is: /home/cloud_user

Your History File Will Ignore: ignoredups

Your Terminal Session Type is: xterm-256color
```

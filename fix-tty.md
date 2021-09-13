Spawning bash with python:

```
$ python -c 'import pty; pty.spawn("/bin/bash")'
```

Background'ing the remote shell with CTRL-Z:

```
user@remote:~$ ^Z
```

Getting ROWS and COLS within current terminal window:

```
user@local:~$ stty -a | head -n1 | cut -d ';' -f 2-3 | cut -b2- | sed 's/; /\n/'
```

Ignoring hotkeys in the local shell and getting back to the remote:

```
user@local:~$ stty raw -echo; fg
```

Setting correct size for the remote shell (where ROWS and COLS are the values from the 3rd bullet):

```
user@remote:~$ stty rows ROWS cols COLS
```

Adding some colors:

```
user@remote:~$ export TERM=xterm-256color
```

Reloading bash to apply the TERM variable:
```
user@remote:~$ exec /bin/bash
```

Src: https://forum.hackthebox.eu/discussion/142/obtaining-a-fully-interactive-shell

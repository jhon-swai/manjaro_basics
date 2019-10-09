# Common terminal commands that are worth knowing in any distribution for begginers.

All of the basic commands for which much information is available elsewhere:
ls, mv, cp, cd, rm, rmdir, mkdir

Commands you should learn to use that have entire guides dedicated to their usage:
find, grep, less, ps, chown, chmod

### Show a list of your disks and partitions
```
lsblk
```

### Show all your mounted partitions, how much space is used and how much is free:
```
df -h
```

### Shutdown the system
```
systemctl poweroff
```

### Reboot
```
systemctl reboot
```

### List all the potential systemd unit files
```
systemctl list-unit-files
```

### Start/stop/enable/disable a service:
replace with any of the above
```
systemctl start <service>
```
example
```
sudo systemctl restart apache2
```

### Get information about a command:
```
which <command>
```

### Get help on the usage of a command:
```
man <command>
```

### Dump the contents of a file to the screen:
```
cat <filename>
```

### Run a command as root or another user:
```
sudo <command>
```

# PACMAN
 Pacman is the package manager from upstream Arch linux.
 Pacman includes some advanced features not in pamac
 
### Installing updates 
```
sudo pacman -Syu
```
### Searching for packages 
```
pacman -Ss <any-keyword>
```
### Searching installed packages 
```
pacman -Qs <any-keyword>
```
### List all installed packages 
```
pacma -Ql
```
### installing packages
```
sudo pacman -Syu <package-name>
```
 note: 'yu' is for updating the package '-S' alone could be enough to download.
### installing packages from the local system
```
sudo pacman -U <package-location>
```
or could be from the internet 
```
sudo pacman -U <address>
```
### Removing packages
```
sudo pacman -R <package-name>
```
to remove the package with all the unneeded dependencies
```
sudo pacman -Rsu <package-name>
```
### Viewing and removing orphans 
orphans are installed packages that are not used by anything els
To list them
```
pacman -Qdt
```
To remove them all
```
sudo pacman -Rs $(pacman -Qdtq)
```
### Downloading packages without installing 
The downloaded package will be stored at /var/cache/pacman/pkg
```
sudo pacman -Sw <package-name>
```

### Cache management
When pacman installs packages, it keeps a copy of all the old packages you have downloaded. 

 To clear cache of packages that are no longer installed 
```
sudo pacman -Sc
```
 To clear cache completely
```
sudo pacman -Scc
```
 Safe way to remove old packages 

```
paccache -rvk3
```

### pacman.conf
Location: /etc/pacman.conf
Case sensitive: yes 

##### Enabling color 
uncomment Color

##### Pacman eating power pills 
Add the line ILoveCandy


## next is [pacman troubleshouting](https://wiki.manjaro.org/index.php?title=Pacman_troubleshooting)



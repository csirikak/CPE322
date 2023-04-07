## Lab 2 — Command Line
Run on Debian WSL
### hostname
Prints the hostname of the device
```
$ hostname
Kregler
```
### env
Shows the environment variables
```
$ env
SHELL=/bin/bash
WSL_DISTRO_NAME=Debian
NAME=Kregler
PWD=/home/nj
LOGNAME=nj
HOME=/home/nj
LANG=en_US.UTF-8
WSL_INTEROP=/run/WSL/8_interop
LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.webp=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:
WAYLAND_DISPLAY=wayland-0
TERM=xterm-256color
USER=nj
DISPLAY=:0
SHLVL=1
XDG_RUNTIME_DIR=/mnt/wslg/runtime-dir
WSLENV=
PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/usr/lib/wsl/lib:/mnt/c/Program Files (x86)/Common Files/Oracle/Java/javapath:/mnt/c/Windows/system32:/mnt/c/Windows:/mnt/c/Windows/System32/Wbem:/mnt/c/Windows/System32/WindowsPowerShell/v1.0/:/mnt/c/Windows/System32/OpenSSH/:/mnt/c/Program Files (x86)/NVIDIA Corporation/PhysX/Common:/mnt/c/Program Files/NVIDIA Corporation/NVIDIA NvDLISR:/mnt/c/WINDOWS/system32:/mnt/c/WINDOWS:/mnt/c/WINDOWS/System32/Wbem:/mnt/c/WINDOWS/System32/WindowsPowerShell/v1.0/:/mnt/c/WINDOWS/System32/OpenSSH/:/mnt/c/ProgramData/chocolatey/bin:/mnt/c/Users/n_j/AppData/Roaming/nvm:/mnt/c/Program Files/nodejs:/mnt/c/Program Files/Git/cmd:/mnt/c/Program Files/dotnet/:/mnt/c/Program Files/PuTTY/:/mnt/c/Program Files/Docker/Docker/resources/bin:/mnt/c/ProgramData/DockerDesktop/version-bin:/mnt/c/Users/n_j/AppData/Roaming/Python/Python310/Scripts:/mnt/c/Program Files/PowerShell/7/:/mnt/c/Users/n_j/AppData/Local/Programs/Python/Python310/:/mnt/c/users/n_j/appdata/local/programs/python/python310/lib/site-packages:/mnt/c/Program Files/mosquitto:/mnt/c/Users/n_j/AppData/Local/Programs/Python/Python310/Scripts/:/mnt/c/Users/n_j/AppData/Local/Microsoft/WindowsApps:/mnt/c/Users/n_j/AppData/Local/Programs/Microsoft VS Code/bin:/mnt/c/msys64/mingw64/bin:/mnt/c/Users/n_j/AppData/Roaming/npm:/mnt/c/Program Files (x86)/Nmap:/mnt/c/msys64/mingw64/include/opencv4:/mnt/c/Users/n_j/Downloads/eda/ghdl:/mnt/c/Users/n_j/Downloads/eda/gtkwave64
HOSTTYPE=x86_64
PULSE_SERVER=/mnt/wslg/PulseServer
_=/usr/bin/env
OLDPWD=/home/nj/demo
```
### ps
Shows a list of running processes
```
$ ps
  PID TTY          TIME CMD
    9 pts/0    00:00:00 bash
   40 pts/0    00:00:00 ps
```
### pwd
Shows the current working directory
```
$ pwd
/home/nj
```
### git clone
Clones a github repository onto the local system
```
$ git clone https://github.com/kevinwlu/iot.git
Cloning into 'iot'...
remote: Enumerating objects: 18743, done.
remote: Counting objects: 100% (1457/1457), done.
remote: Compressing objects: 100% (512/512), done.
remote: Total 18743 (delta 814), reused 1282 (delta 720), pack-reused 17286
Receiving objects: 100% (18743/18743), 27.63 MiB | 10.32 MiB/s, done.
Resolving deltas: 100% (12545/12545), done.
```
### cd
Changes the working directory, enter alone to return to the home directory
```
$ cd iot
~/iot$
```
### ls
Lists files and folders in the current directory
```
$ ls
apps       health   lesson10  lesson4  lesson7  make       special_problems
cases      hype     lesson2   lesson5  lesson8  projects   standards
economics  lesson1  lesson3   lesson6  lesson9  README.md  tools
```
### df
Lists file system disk usage, append -h to make the output more readable
```
$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sdc        251G  1.3G  237G   1% /
none            3.7G   44K  3.7G   1% /mnt/wslg
none            3.7G  4.0K  3.7G   1% /mnt/wsl
tools           931G  326G  606G  35% /init
none            3.7G     0  3.7G   0% /dev
none            3.7G     0  3.7G   0% /run
none            3.7G     0  3.7G   0% /run/lock
none            3.7G     0  3.7G   0% /run/shm
none            3.7G     0  3.7G   0% /run/user
tmpfs           3.7G     0  3.7G   0% /sys/fs/cgroup
drivers         931G  326G  606G  35% /usr/lib/wsl/drivers
lib             931G  326G  606G  35% /usr/lib/wsl/lib
none            3.7G   76K  3.7G   1% /mnt/wslg/versions.txt
none            3.7G   76K  3.7G   1% /mnt/wslg/doc
drvfs           931G  326G  606G  35% /mnt/c
```
### mkdir
Creates a new directory with the given name/path
```
$ mkdir demo
$ cd demo
~/demo$
```
### nano
Opens a file with a given name in a console editor
```
$ nano file
I like trains
CTRL-X
Y
Enter
```



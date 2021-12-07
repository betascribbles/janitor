# unix-janitor
This is a simple sript that lets you update, upgrade and clean your linux distro with a single command that you can run anywhere in your terminal.

## Requirements to use this script
- Use a linux distro
- Have `sudo` privileges
- Locate the `$PATH` folder
- Ensure the file `janitor` has excecutable permissions
- Be patient!!

## How to use this script
- Clone this repo to your local machine
```
beta@firdaus-pc:~$ git clone https://github.com/betascribbles/unix-janitor.git
Cloning into 'unix-janitor'...
remote: Enumerating objects: 13, done.
remote: Counting objects: 100% (13/13), done.
remote: Compressing objects: 100% (13/13), done.
remote: Total 13 (delta 2), reused 5 (delta 0), pack-reused 0
Unpacking objects: 100% (13/13), 2.97 KiB | 759.00 KiB/s, done.
beta@firdaus-pc:~/Documents$ 
```

- Change into the repo directory
```
beta@firdaus-pc:~$ ls
unix-janitor
beta@firdaus-pc:~$ cd unix-janitor/
beta@firdaus-pc:~/unix-janitor$
```

- Locate the file `janitor` and copy it to your $PATH folder. <b> This will prompt for the root password</b>
```
beta@firdaus-pc:~/unix-janitor$ ls
janitor  LICENSE  README.md
beta@firdaus-pc:~/unix-janitor$ sudo cp janitor /usr/bin/
[sudo] password for beta: 
beta@firdaus-pc:~/unix-janitor$ 
```

- You can update, upgrade and clean-up your linux distro but running `janitor` anywhere in your terminal
```
beta@firdaus-pc:~/Documents/FIRDAUS/$ janitor
 Step 1: Updating packages
===========================
Hit:1 https://brave-browser-apt-release.s3.brave.com stable InRelease   
Hit:2 http://packages.microsoft.com/repos/code stable InRelease                                        
Hit:3 https://dl.google.com/linux/chrome/deb stable InRelease                                          
Hit:4 http://ke.archive.ubuntu.com/ubuntu focal InRelease
Hit:5 http://ke.archive.ubuntu.com/ubuntu focal-updates InRelease
Hit:6 http://ke.archive.ubuntu.com/ubuntu focal-backports InRelease
Hit:7 http://security.ubuntu.com/ubuntu focal-security InRelease
Reading package lists... Done

 Step 2: Upgrading packages
============================
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Calculating upgrade... Done
The following packages have been kept back:
  fwupd fwupd-signed gnome-shell-extension-desktop-icons libegl-mesa0 libfwupd2 libfwupdplugin1 libgbm1 libgl1-mesa-dri libglapi-mesa libglx-mesa0
  libsmbclient libwbclient0 libxatracker2 linux-generic-hwe-20.04 linux-headers-generic-hwe-20.04 linux-image-generic-hwe-20.04 mesa-vulkan-drivers
  samba-libs ubuntu-advantage-tools
0 upgraded, 0 newly installed, 0 to remove and 19 not upgraded.

 Step 3: Repair broken dependencies
==================================
Reading package lists... Done
Building dependency tree       
Reading state information... Done
 Step 4: Removing all the junk files
=====================================
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Reading package lists... Done
Building dependency tree       
Reading state information... Done
0 upgraded, 0 newly installed, 0 to remove and 19 not upgraded.

beta@firdaus-pc:~/Documents/FIRDAUS/ALX/unix-janitor$ 
```
- Tada! Your operating system thanks you for cleaning it up!!

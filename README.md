# unix-janitor
This is a simple sript that lets you update, upgrade and clean your linux distro with a single command that you can run anywhere in your terminal.

## Requirements to use this script
1. Use a linux distro
2. Have `sudo` privileges
3. Locate the `$PATH` folder
4. Be patient!!

## How to use this script
1. Clone this repo to your local machine
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

2. Change into the repo directory
```
beta@firdaus-pc:~$ ls
unix-janitor
beta@firdaus-pc:~$ cd unix-janitor/
beta@firdaus-pc:~/unix-janitor$
```

3. Locate the file `janitor` and copy it to your $PATH folder. <b> This will prompt for the root password</b>
```
beta@firdaus-pc:~/unix-janitor$ ls
janitor  LICENSE  README.md
beta@firdaus-pc:~/unix-janitor$ sudo cp janitor /usr/bin/
[sudo] password for beta: 
beta@firdaus-pc:~/unix-janitor$ 
```

4. You can update, upgrade and clean-up your linux distro but running `janitor` anywhere in your terminal
```
beta@firdaus-pc:~/Documents/FIRDAUS$ janitor
 Step 1: Upgrading your distro
==============================
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Calculating upgrade... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.

 Step 2: Updating packages
===========================
Hit:1 https://brave-browser-apt-release.s3.brave.com stable InRelease 
Hit:2 http://ke.archive.ubuntu.com/ubuntu focal InRelease             
Hit:3 http://ke.archive.ubuntu.com/ubuntu focal-updates InRelease                                                                                    
Hit:4 http://ke.archive.ubuntu.com/ubuntu focal-backports InRelease                                                                                  
Hit:5 https://dl.google.com/linux/chrome/deb stable InRelease                                                                       
Hit:6 http://packages.microsoft.com/repos/code stable InRelease     
Hit:7 http://security.ubuntu.com/ubuntu focal-security InRelease
Reading package lists... Done

 Step 3: Upgrading packages
============================
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Calculating upgrade... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.

 Step 4: Repair broken dependencies
====================================
Reading package lists... Done
Building dependency tree       
Reading state information... Done

 Step 5: Removing all the junk files
=====================================
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Reading package lists... Done
Building dependency tree       
Reading state information... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.

 	CONGRATULATIONS!!
 	Your system is clean and up-to-date

beta@firdaus-pc:~/Documents/FIRDAUS$ 
```
Tada! Your operating system thanks you for cleaning it up!!

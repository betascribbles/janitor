# janitor
### Shell Script: Automate Linux Updates, Upgrades and Clean-up Operations
A janitor is one who keeps the premises of a building (such as an apartment or office) clean, tends the premises' system, and makes minor repairs. This is a simple shell script to automate all the cleaning, updating, and taking care of your system.

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

4. You can update, upgrade and clean-up your linux distro but running `janitor` anywhere in your terminal.
```
beta@firdaus-pc:~/unix-janitor$ ./janitor 
 Step 1: Updating|Upgrading packages
=====================================
[sudo] password for beta: 
Hit:1 https://brave-browser-apt-release.s3.brave.com stable InRelease    
Hit:2 http://ppa.launchpad.net/apandada1/brightness-controller/ubuntu focal InRelease
Hit:3 http://archive.ubuntu.com/ubuntu focal InRelease                   
Hit:4 https://download.docker.com/linux/ubuntu focal InRelease           
Hit:5 http://apt.puppetlabs.com focal InRelease
Reading package lists... Done
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Calculating upgrade... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.

 Step 3: Repair broken packages/dependencies
=============================================
Hit:1 http://ppa.launchpad.net/apandada1/brightness-controller/ubuntu focal InRelease
Hit:2 https://brave-browser-apt-release.s3.brave.com stable InRelease    
Hit:3 https://download.docker.com/linux/ubuntu focal InRelease           
Hit:4 http://archive.ubuntu.com/ubuntu focal InRelease                   
Hit:5 http://packages.microsoft.com/repos/code stable InRelease
Fetched 336 kB in 5s (73.5 kB/s)
Reading package lists... Done
Building dependency tree       
Reading state information... Done
10 packages can be upgraded. Run 'apt list --upgradable' to see them.
Hit:1 https://download.docker.com/linux/ubuntu focal InRelease           
Hit:2 https://brave-browser-apt-release.s3.brave.com stable InRelease    
Hit:3 http://archive.ubuntu.com/ubuntu focal InRelease                   
Hit:4 http://ppa.launchpad.net/apandada1/brightness-controller/ubuntu focal InRelease
Hit:5 https://deb.nodesource.com/node_14.x focal InRelease
Fetched 336 kB in 5s (71.3 kB/s)
Reading package lists... Done
Reading package lists... Done
Building dependency tree       
Reading state information... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.

 Step 4: Removing all the junk files
=====================================
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Reading package lists... Done
Building dependency tree       
Reading state information... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.

 Last step: Updating packages
==============================
Hit:1 https://download.docker.com/linux/ubuntu focal InRelease           
Hit:2 http://ppa.launchpad.net/apandada1/brightness-controller/ubuntu focal InRelease
Hit:3 https://brave-browser-apt-release.s3.brave.com stable InRelease    
Hit:4 https://dl.google.com/linux/chrome/deb stable InRelease            
Hit:5 http://apt.puppet.com bionic InRelease
Fetched 336 kB in 6s (53.5 kB/s)                                         
Reading package lists... Done
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Calculating upgrade... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.

 	CONGRATULATIONS beta!!
 	Your system is clean and up-to-date

beta@firdaus-pc:~/unix-janitor$ 
```
Tada! Your operating system thanks you for cleaning it up!!

----
See [Wiki page](https://github.com/betascribbles/janitor/wiki/How-to-Take-Care-of-Your-LinuxOS-with-janitor) for more info about janitor.

Feel free to contribute in making the script better.

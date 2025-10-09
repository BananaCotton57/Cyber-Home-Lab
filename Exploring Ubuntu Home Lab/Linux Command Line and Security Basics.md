## 1. Searching for Available Updates

**Command:**
```bash
apt list --upgradable 
```

This command lists all the packages on my system that have available updates. For each package, it shows:

- Package name - The software package that can be updated.

- Repository - The source where the updated package comes from.

- Architecture - The system type this update applies to.

- Current version - The version current installed.

- New version - The version available in the repository that can be installed

![List of Upgradeable Packages](images/image1.png)

### For the second listing:

- The package name is landscape-common.

- The repository is jammy-updates.

- The architecture this update is available is arm64.systems

- The current version of this package is 23.02-0ubuntu1-22.04.4

- The new version of this package is 23.02-0ubuntu1-22.04.6

## 2. Updating and Upgrading the System

**Command (update):**
```bash
sudo apt update
```

Using this command will download the latest package information from all my configured sources. This command will not upgrade any of those packages.

![Command to Update](images/image2.png)

**Command (upgrade):**
```bash
sudo apt upgrade
```

This command will install all packages to their latest versions based on the updated package list.

![Command to Upgrade](images/image3.png)

**Note:**

One package, ```cloud-init```, was shown as "*held back.*" This is normal behavior for virtual machines and can be ignored.

## 3. Rebooting the System

**Command:**
```bash 
sudo reboot
```

This command restarts my system. It is also usually necessary to run it to ensure all updates were fully applied.

# Users and Permissions

## 4. Changing to the Root User

**Command:**
```bash
sudo su root
```

Using this command switches the current user, ```ngoj```, to the root user. The prompt of the root user has a different color and style from a normal user, and it also is indicated by a ```#``` instead of ```$```.

![Root User](images/image4.png)

## 5. Creating New Users

There are two options to create a new user in Linux:

**Command 1:**
```bash
sudo useradd username
```

**Command 2:**
```bash
sudo adduser username
```

The first option, `sudo useradd username`,
is a built in Linux Command that directly adds a new user to the /etc/passwd file, but it does not create a home directory or a password for the user. 

The second option, `sudo adduser username`,
is a Perl script that utilizes useradd, and it guided me through creating a home directory and a password for the new user.


![useradd and adduser](images/image5.png)


# 1. Searching for Available Updates

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

![List of upgradeable packages](images/image1.png)

### For the second listing:

- The package name is landscape-common.

- The repository is jammy-updates.

- The architecture this update is available is arm64.systems

- The current version of this package is 23.02-0ubuntu1-22.04.4

- The new version of this package is 23.02-0ubuntu1-22.04.6

# 2. Updating and Upgrading the system

**Command for updating:**
```bash
sudo apt update
```

Using this command will download the package information from all my configured sources.

![Command to update](images/image2.png)

**Command for upgrading:**
```bash
sudo apt upgrade
```

This command will act on the downloaded information and upgrade all packages to their latest versions.

![Command to Upgrade](images/image3.png)
# Gcc-guide

This guide provides instructions for installing, updating, and changing the version of the GCC compiler on Ubuntu.
Installing GCC
Method 1: Using apt

 1. Install GCC:

### bash
   
    sudo apt install gcc

This command installs the default version of GCC available in the Ubuntu repository.

Verify the Installation:

bash

    gcc --version

This command displays the installed GCC version.

Method 2: Installing a Specific Version

 If you require a specific version of GCC, follow these steps:

 Check Available Versions:

bash

    apt search gcc

Install a Specific Version:

bash

    sudo apt install gcc-<version_number>

Replace <version_number> with the specific version you want to install (e.g., gcc-9, gcc-10, etc.).
 Verify the Installation:
    
      gcc --version

Changing GCC Version

To switch between installed GCC versions:

Navigate to the GCC directory:

bash

    cd /usr/bin

List the installed GCC versions:

bash

    ls

Remove the existing version:

bash

    sudo rm gcc

Update the version:

bash

    sudo cp gcc<version> gcc

Replace <version> with the desired version.
Updating GCC

To update GCC to the latest available version:

Update GCC:

bash

    sudo apt upgrade gcc

This command upgrades GCC to the latest version available in the Ubuntu repository.

    Verify the Updated Version:

bash

    gcc --version

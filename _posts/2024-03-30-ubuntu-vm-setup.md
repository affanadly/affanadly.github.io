---
layout: post
title: Setting up a Ubuntu 22.04 LTS VM in Oracle Virtualbox
date: 2024-03-30 12:00:00
tags: vm linux setup
categories: guide
---

This is how I setup my Ubuntu 22.04 LTS VM every time I need to work on a fresh installation.

## Pre-Installation

1. Load the Ubuntu 22.04 LTS ISO file when initializing the new VM, but disable the unattended installation.
2. Allocate (at least) 2 CPU cores and 4 GB of RAM.
3. Create a new virtual hard disk with a size of (at least) 25 GB.

## During Installation

1. Select the US-US keyboard layout.
2. Select the minimal installation option.
3. Select the Kuala Lumpur, Malaysia region.
4. By default, I set the passwords of my VM to 0000 and enable automatic login.

## Post-Installation

1. Skip the Ubuntu Pro subscription.
2. Disable sending system information to Canonical.
3. Remove Ubuntu softwares and Help from the favourites bar, and move the home folder shortcut to the top-right.
4. Go to the settings and enable the following:
   1. Power: Set blank screen to never
   2. Appearance: Dark mode
   3. Language & Region: Set the language format to UK (requires reboot and login)
5. Install the following packages:

    ```bash
    sudo apt update
    sudo apt install build-essential dkms linux-headers-$(uname -r)
    ```

6. Install the Virtualbox Guest Additions Disk and run the autorun script.
7. Add the current user to the vboxsf group:

    ```bash
    sudo adduser $USER vboxsf
    ```

8. Reboot the VM.
9. Eject the Virtualbox Guest Additions Disk.
10. Enable bidirectional shared clipboard and add shared folders if necessary.
11. Update all softwares:

    ```bash
    sudo apt upgrade
    ```

12. Shut down and create a snapshot of the fresh VM.

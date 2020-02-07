# ClearWSL
Clear Linux on WSL (Windows 10 x64 1709 (Fall Creators Update) or later)
based on [wsldl](https://github.com/yuk7/wsldl)

![screenshot](https://raw.githubusercontent.com/wiki/yuk7/wsldl/img/Cent_Arch_Alpine.png)
[![Build Status](https://img.shields.io/travis/com/wight554/ClearWSL.svg?style=flat-square)](https://travis-ci.com/wight554/ClearWSL)
[![Github All Releases](https://img.shields.io/github/downloads/wight554/ClearWSL/total.svg?style=flat-square)](https://github.com/wight554/ClearWSL/releases/latest)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
![License](https://img.shields.io/github/license/wight554/ClearWSL.svg?style=flat-square)

### [Download](https://github.com/wight554/ClearWSL/releases/latest)


## Requirements
* Windows 10 1709 Fall Creators Update x64 or later.
* Windows Subsystem for Linux feature is enabled.

## Install
#### 1. [Download](https://github.com/wight554/ClearWSL/releases/latest) installer zip

#### 2. Extract all files in zip file to same directory

#### 3. Run Clear.exe to Extract rootfs and Register to WSL
Exe filename is used to register the instance name.
If you rename it, you can register with a different name and have multiple installs.


## How-to-Use(for Installed Instance)
#### exe Usage
```dos
Usage :
    <no args>
      - Open a new shell with your default settings.

    run <command line>
      - Run the given command line in that distro. Inherit current directory.

    config [setting [value]]
      - `--default-user <user>`: Set the default user for this distro to <user>
      - `--default-uid <uid>`: Set the default user uid for this distro to <uid>
      - `--append-path <on|off>`: Switch of Append Windows PATH to $PATH
      - `--mount-drive <on|off>`: Switch of Mount drives

    get [setting]
      - `--default-uid`: Get the default user uid in this distro
      - `--append-path`: Get on/off status of Append Windows PATH to $PATH
      - `--mount-drive`: Get on/off status of Mount drives
      - `--lxuid`: Get LxUID key for this distro

    backup
      - Output backup.tar.gz to the current directory using tar command.
      
    clean
      - Uninstall the distro.

    help
      - Print this usage message.
```


#### How to uninstall instance
```dos
>Clear.exe clean

```

[![Maintenance](https://img.shields.io/maintenance/yes/2024.svg)]()
# ctOS-Repo
Repository for ctOS packages

## Installation 
Edit the following lines to your /etc/pacman.conf
```
[ctOS]
SigLevel = Optional DatabaseOptional
Server = https://raw.githubusercontent.com/whatev33r/ctOS-Repo/master/$arch
```

## PKGBUILDS for ctOS
The source PKGBUILD files contained in the ctOS repository are found in the [packages](/packages) folder.

> **devtools** package is requied to build packages!

## Build Preparation
Build Script has to be executed as **user**!
```
sudo chown -R <user>:<user> . 
```

## Build Script
Build **every** Package:
```
./build.sh
```
Build **single** Package:
```
./build.sh "<package_name>"
```

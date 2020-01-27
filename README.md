#zenpower-dkms
This repository contains a Debian-ready package for [ocerman's zenpower module](https://github.com/ocerman/zenpower "ocerman's zenpower module"). Zenpower is added as submodule, the `dkms` file in `debian/` is just a symlink and every change I made comes as a quilt patch. Additionally there's a `zenpower.conf` which blacklists the interfering k10temp module. I've even prepared a .deb package for lazy people like me ;)
##Installation
- Clone this repository
- Update submodule if necessary
- Build package with `dpkg-buildpackage -us -uc -b`
- Install package and enjoy your new sensors

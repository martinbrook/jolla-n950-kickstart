jolla-n950-kickstart
====================

This comes with no warranty. Hardware adaptation can destroy your device

A WIP kickstart for Nokia N950 pulling from Jolla repos

You will need

Mer Plaform SDK - https://wiki.merproject.org/wiki/Platform_SDK

Nemomobile N950 Installation Instructions - https://wiki.merproject.org/wiki/Nemo/Installing


Using the platform sdk create a filesystem image 

sudo mic create fs jolla-n950-kickstart.ks -o . --pkgmgr=zypp --arch armv7hl  --pack-to=vgrade-sailfish.tar.bz2

Flash to N950

sudo tar --numeric-owner -xjf vgrade-sailfish.tar.bz2 -C /mnt



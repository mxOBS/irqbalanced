Russell King's irqbalanced fork for ARM devices
===============================================

This is a fork of irqbalanced to add proper support for ARM devices.
The regular irqbalanced contains several IRQ misclassifications, which renders it useless
on these systems. Also, the way the number of CPUs were being determined was faulty.

The sources are hosted here with Russell King's permission, to make it easier to build irqbalanced with Yocto, for example.

Building follows the regular autotools pattern, which is:

    ./autogen.sh
    ./configure
    make
    make install

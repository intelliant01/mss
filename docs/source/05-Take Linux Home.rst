Take Linux Home
===============

Create Live USB
-----------------
Li-f-e: Linux for Education OS image is included on the server and can
be used to create a bootable media when logged in as **mssadmin** user.

:Note: When creating a bootable media intended to boot computers that only
    support EFI booting, select "isohybrid" option. This option can also boot
    on legacy hardware so use this if you are not sure about your hardware
    capabilities. Use of "isohybrid" option is officially recommended way of
    creating bootable USB. *Do note that this will wipe the USB device and
    cannot be used as a normal storage media from Windows PC.* 
    
    Use "Ubuntu" or "Legacy" option if you wish to use the device as a storage media on Windows or
    preserve data on a vfat formatted USB stick.

Via Shortcuts
^^^^^^^^^^^^^

Use either of these launcher icons on the Desktop - ``Live USB GUI EFI`` or ``Live USB GUI Legacy`` as per your bootable media preference.

Via Menu
^^^^^^^^
::

  System Tools -> Live USB GUI

You will be requested for the ISO image in the above process. The same is located at either of these directory paths - ``/recovery/`` or ``/home/mssadmin/``

Via Terminal
^^^^^^^^^^^^

It may be more convenient to use command line for running this task multiple
times.

::

    sudo live-grub-stick --isohybrid /recovery/Li-f-e.iso /dev/sdb

Guide & Troubleshoot
^^^^^^^^^^^^^^^^^^^^
See the following external links *(requires internet)* to learn how to boot from USB stick and
troubleshoot if the USB does not boot:

`Change the boot order in BIOS<https://www.lifewire.com/change-the-boot-order-in-bios-2624528>`__

`Boot from a USB device<https://www.lifewire.com/how-to-boot-from-a-usb-device-2626091>`__
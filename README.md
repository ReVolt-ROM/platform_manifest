ReVolt KK ROM
======================

Syncing Sources
---------------
Intialize your computer by syncing with latest sources via this command :

    repo init -u git://github.com/ReVolt-ROM/platform_manifest.git -b kitkat

then run to get the actual sources

    repo sync -j#

It might take a lot of time depending on your internet connection .. 

 # is replaced with threads you want to use

Building REVOLT ROM (Still not fully ready with KitKat)
------------------------------------------------------


Now you can run the build script:

     . build_revolt.sh DEVICE SYNC CORES CLEAN


- Device: Write the code-name of your device (Must be a supported device)

- Sync: Wether to sync latest source or not before the actual build

- Cores: Allows to choose number of cores of processor to use during the build

- Clean: Clean the previous build data to start a fresh clean build

Examples:

    . build_revolt.sh mako sync 9 noclean

(This will sync latest sources, Use 9 cores, Not Clean & build Revolt for the Nexus 4)

    . build_revolt.sh i9100 nosync 4 clean

(This will not sync source, use 4 cores, clean and build Revolt for the I9100)



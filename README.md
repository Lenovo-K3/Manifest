Manifest
================

Local Manifest to build CyanogenMod for Lenovo K30-T

Build Instructions
-----------------------------------------------------------------------------
1. Install build software for Ubuntu:

		sudo apt-get install bison build-essential curl flex lib32ncurses5-dev lib32readline-gplv2-dev lib32z1-dev libesd0-dev libncurses5-dev libsdl1.2-dev libwxgtk2.8-dev libxml2 libxml2-utils lzop openjdk-7-jdk openjdk-7-jre pngcrush schedtool squashfs-tools xsltproc zip zlib1g-dev git-core make phablet-tools gperf

2. Initialize repo:
    
		repo init -u git://github.com/CyanogenMod/android.git -b cm-13.0

3. Add my local manifest

		mkdir .repo/local_manifests
		Copy manifest.xml to .repo/local_manifests

4. Then sync up the repositories

		repo sync

5. Initialize the build environment

		source build/envsetup.sh
    
6. Build the ROM

		lunch / make / brunch

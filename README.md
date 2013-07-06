Local manifests to build CyanogenMod 10.1 for Xiaomi MI-One.

How to build:
-------------

Initialize repo:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-10.1
    curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/mirom/android_local_manifest/cm-10.1/local_manifest.xml
    repo sync

    . build/envsetup.sh
    brunch mione_plus

Local manifests to build CyanogenMod 10.1 for Xiaomi Mi2.

编译方法:
-------------

1、repo init -u git://github.com/CyanogenMod/android.git -b cm-10.1

2、curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/mitwo/android_local_manifest/cm-10.1/local_manifest.xml

3、repo sync

4、. build/envsetup.sh

5、brunch aries

Local manifests to build CyanogenMod 10.1 for Xiaomi Mi2.

编译方法:
-------------

1、建立cm-10.1源码树：
repo init -u git://github.com/CyanogenMod/android.git -b cm-10.1

2、建立mi2特定local_manifests：
curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/mitwo-dev/android_local_manifest/cm-10.1/local_manifest.xml

3、开始同步源码：
repo sync

4、开始编译：
. build/envsetup.sh
brunch aries

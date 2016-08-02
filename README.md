
How to build:
-------------

Initialize repo:

    repo init -u git://github.com/omnirom/android.git -b android-6.0 --depth 1
    curl --create-dirs -L -o .repo/local_manifests/local_manifests.xml -O -L https://raw.githubusercontent.com/BambooIV/android_local_manifests/android-6.0/manifests_zte_nx503a.xml
    repo sync -j16

Compile:

    . build/envsetup.sh
    breakfast nx503a
    make bacon -j4

Note:
-------------
Not working:

    Audio
    Baseband
    Camera
    etc.

This is a memo for compilation of omnirom.

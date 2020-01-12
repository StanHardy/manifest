# Bliss Q

![zuk_z2](https://github.com/magicxavi/manifest/raw/blissQ-zuk/BLISS%20ROM_Lenovo%20ZUK%20Z2.png "zuk_z2")

Synch sources:

    $ repo init -u https://github.com/BlissRoms/platform_manifest.git -b q
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/magicxavi/manifest/blissQ-zuk/bliss.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Zuk Z2/Z2 Plus
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch bliss_z2_plus-userdebug
    $ make blissify

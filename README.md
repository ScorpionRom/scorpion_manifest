# ScorpionROM
------------------

Getting Started
------------------

To get started with building Scorpion Rom, you'll need to get familiar with Git and Repo.

Setting up the Build Environment:
You can use this [Guide](https://raw.githubusercontent.com/nathanchance/Android-Tools/master/Guides/Building_AOSP.txt) by nathanchance, there's also a [Guide](https://scorpionrom.com/building-scorpionrom-with-manjaro-linux) on our website specifically for building ScorpionROM using Manjaro Linux.

Initialize Source:

        mkdir srx (or whatever you want to name the source folder)

        cd ~/srx

        repo init -u https://github.com/ScorpionRom/scorpion_manifest.git -b sr5

Sync Source:

        repo sync -c -j16 --force-sync --no-clone-bundle --no-tags

Build Source:

        . build/envsetup.sh
        lunch scorpion_crosshatch-userdebug (or whichever device you are building for, change out "crosshatch")
        make clean
        make bacon

Submitting Patches
------------------
We're open source, and patches are always welcome!

You can push to our Gerrit server: https://gerrit.scorpionrom.com


Credits:

Google for AOSP

Everyone at Dirty Unicorns

Ezio at ABC

Rinky McBally for our beloved logo

Moelle for the amazing boot animation

ROGERdotT (Roger Truttmann) for the v3.x wallpapers

Others we may have missed

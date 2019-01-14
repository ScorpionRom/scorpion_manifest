Scorpion
------------------

Getting Started
------------------

To get started with building Scorpion Rom, you'll need to get familiar with Git and Repo.

Initialize Source (Assuming you have a valid build environment setup):

        mkdir scorpion (or whatever you want to name the source folder)

        cd ~/scorpion
        repo init -u https://github.com/ScorpionRom/manifest.git -b test

Sync Source:

        repo sync -c -f -jx --force-sync --no-clone-bundle --no-tags (x being however many cpu jobs, you can also use -c to sync only the current branch specified by repo init)

Build Source:

        . build/envsetup.sh
        lunch scorpion_device-userdebug (device should be device codename ie:cheeseburger, dumpling, angler, etc..)
        mka clean
        mka bacon
Submitting Patches
------------------
We're open source, and patches are always welcome!

At this time we do not have a gerrit server, but are open to the idea in the future. For now submit patchs by doing a pull request.


Credits:

Google for AOSP

InvictrixRom

Lineage OS

Rinky McBally for our beloved logo and Wallpapers

Others we may have missed


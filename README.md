# Hycon OS #
<img src="https://i.postimg.cc/NG3S1xdM/Pics-Art-01-20-07-06-57.png">

Credits:
=======
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**RevengeOS**](https://github.com/RevengeOS)
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**DirtyUnicorns**](https://github.com/dirtyunicorns)
 * [**AospExtended**](https://github.com/AospExtended)
 * [**ABC**](https://github.com/ezio84?tab=repositories)
 * [**Project-Awaken**](https://github.com/Project-Awaken)
 * [**PixelExtended**](https://github.com/PixelExtended)
 * [**WaveOS**](https://github.com/Wave-Project)

-----------------------------------------------------------------------------

### Getting Started: ###

To initialize your local repository, use a command like this:
```bash
repo init -u https://github.com/HyconOS/manifest -b eleven
```

### Then to sync up: ###

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Finally to build: ###

From root directory of Project, perform following commands in terminal:
```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```
# XDA Template
[![XDA-Template](https://i.postimg.cc/rp82Qf02/XDADevelopers-button.png)](https://raw.githubusercontent.com/HyconOS/manifest/eleven/Xda)

### Maintainership ###
If You wish to maintain Hycon OS For your device Officially , Contact @Prophecy_Child or @introdructor on telegram.

Some things to consider before applying:

• You must own the device. Blind and untested builds aren't allowed.

• You must have knowledge of git.

• You must do one or two unofficial build[Post at XDA], be sure that the build is stable for daily usage before applying. Stability context may differ for different devices, so explain for any exceptions.

• You must have your device sources public [Modified trees needed] .

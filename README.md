# Hycon OS #
<img src="https://github.com/Introdructor/images/raw/main/20210607_173402.png">

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
 * [**Evolution-X**](https://github.com/Evolution-X)

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
## Setting up your build environment ##
To set up your build environment please follow this guide: [Link](https://raw.githubusercontent.com/nathanchance/Android-Tools/master/Guides/Building_AOSP.txt)

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
If You wish to maintain Hycon OS For your device Officially , apply through our maintainership form

[![Maintainer-Form](https://img.shields.io/badge/maintainership-form-red?style=for-the-badge&logo=google)](https://forms.gle/ZPv5AwP3A5uABPmY6)

Contact @Prophecy_Child or @introdructor on telegram for further information. Some things to consider before applying:

• You must own the device. Blind and untested builds aren't allowed.

• You must have knowledge of git.

• You must do one or two unofficial build[Post at XDA], be sure that the build is stable for daily usage before applying. Stability context may differ for different devices, so explain for any exceptions.

• You must have your device sources public [Modified trees needed].

## Maintaining Authorship ##
Please make sure if you submit a patch/fix from another ROM that you maintain authorship.
This is very important to not only us but to the entire open source community. It's what keeps it going and encourages more developers to contribute their work.

If you manually cherry pick a patch/fix please add the original author prior to pushing to our Gerrit.
This task is very easy and is usually done after you commit a patch/fix locally.

i.e - Once you type in "git commit -a" the commit message and you have saved it, type in the following:

```bash
git commit --amend --author "Author <email@address.com>"
```

So it should look like this once you get all author's information:

```bash
git commit --amend --author "Alex Cruz <du.alexcruz@gmail.com>"
```

If you do not want to clone or fetch the repo and the patch is on GitHub, you can easily get the author of the patch by adding `.patch` to the end of the commit URL and copy the contents of the lines after the `From:`.

For example: https://github.com/DirtyUnicorns/android_manifest/commit/9d44b2e34fd0b6674de79d001010e513ba14e312.patch

It is also recommended that you keep the date intact as well as it helps other open source users figure out the original version that a patch may have come from. Copy the contents of the date line after the `Date:` then add `--date="<date_just_copied>"` to the above `git commit --amend` command.

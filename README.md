# Shinkai Project AOSP

![Shinkai](https://github.com/Shinkaiprjkt/.github/blob/main/ShinkaiBanner.png?raw=true)

## Getting Started

To get started with the PixelOS source code, you'll need to be
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

To initialize your local repository, run:

```bash
repo init --depth=1 -u https://github.com/Shinkaiprjkt/manifest.git -b hekkaideka --git-lfs
```

Then, sync the repository:

```bash
repo sync --force-sync --no-clone-bundle --no-tags
```

## Building the System

Initialize the ROM build environment by sourcing the envsetup.sh script:

```bash
. b*/env*
```

After cloning the device-specific sources, use breakfast to configure the build for your device:

```bash
breakfast devicecodename
```

Start the compilation:

```bash
m shinkai
```

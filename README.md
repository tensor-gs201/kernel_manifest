# GS201 Kernel Manifest

This is a manifest to sync and build GS201 kernel.

## Setup

Ensure you have repo setup and installed.

```
repo init -u https://github.com/tensor-gs201/kernel_manifest -b thirteen
```

## Sync

```
repo sync --force-sync --optimized-fetch --no-tags --no-clone-bundle -j$(nproc --all)
```

## Build

```
BUILD_CONFIG=private/gs-google/build.config.cloudripper build/build.sh
```


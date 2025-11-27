# Manifest for building Edo's kernel with AOSP Kbuild

## Repo Init ##
```bash
repo init -u https://github.com/realahnet/android_kernel_manifest.git -b master
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```

## Steps ##
- Copy build.config.{pdx206/pdx203} from kernel/msm-4.19 to root of your synced folder for the device you want to build.
- Then run `build/build.sh`

***Note: Change the branch to `master` for non-kernelsu branch of kernel.***

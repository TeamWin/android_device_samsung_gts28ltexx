## TWRP device tree for Samsung Galaxy Tab S2 8.0 (LTE)
## gts28ltexx

Add to `.repo/local_manifests/gts28ltexx.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="ripee/twrp_android_device_samsung_gts28ltexx" path="device/samsung/gts28ltexx" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_gts28ltexx-eng
mka recoveryimage
```

Kernel source: https://github.com/LineageOS/android_kernel_samsung_gts2/tree/cm-14.1

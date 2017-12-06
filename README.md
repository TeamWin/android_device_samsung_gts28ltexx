## TWRP device tree for Samsung Galaxy Tab S2 9.7 (Wi-Fi)
## gts210wifi, gts210wifixx

Add to `.repo/local_manifests/gts210wifi.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="ripee/android_device_samsung_gts210wifi" path="device/samsung/gts210wifi" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_gts210wifi-eng
mka recoveryimage
```


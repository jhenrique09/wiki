## Flashing compatible firmware

1. Download [this](https://wiki-blobs-dl.pixelexperience.org/wiki_blobs_redwood/main/android-12/boot.img) `boot.img` file.
2. Download [this](https://wiki-blobs-dl.pixelexperience.org/wiki_blobs_redwood/main/android-12/dtbo.img) `dtbo.img` file.
3. Download [this](https://wiki-blobs-dl.pixelexperience.org/wiki_blobs_redwood/main/android-12/vendor_boot.img) `vendor_boot.img` file.
4. Power off the device, and boot it into bootloader mode:
    * {{ device.download_boot }}
5. Flash a the downloaded images to your device by typing:
```
fastboot flash vbmeta boot.img
fastboot flash dtbo dtbo.img
fastboot flash vendor_boot vendor_boot.img
```

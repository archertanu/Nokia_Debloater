## Nokia_Debloater
This is Optimised for Nokia 6.1 Plus aka X6.

Nokia 6.1 plus (codenamed _"Dragon"_) is a high-end mid-range smartphone from Nokia/HMD Global.
It was released as the Nokia X6 in the chinese markets.

Nokia 6.1 Plus was announced and released globally on July 2018.

## Device specifications

| Device       |   Nokia 6.1 plus                                |
| -----------: | :---------------------------------------------- |
| SoC          | Qualcomm SDM660 Snapdragon 636                  |
| CPU          | 8x Qualcomm® Kryo™ 260 up to 1.8GHz             |
| GPU          | Adreno 509                                      |
| Memory       | 4GB/6GB                                         |
| Shipped Android version |8.1.0, Oreo                           |
| Current Android version |10.0, Android 10                      |
| Storage      | 64GB eMMC 5.1 flash storage                     |
| Battery      | Non-removable Li-Po 3050 mAh                    |
| Dimensions   | 158.6 x 75.4 x 8.05 mm                          |
| Display      | 2280 x 1080 (18:9), 5.8  inch                   | 

## Get list of system apps on the device:
```bash
adb shell "echo 'apps:' && pm list packages -f | grep /system/app/ | sed 's/.*=/  - /'"
```

## Remove application command
```bash
pm uninstall -k --user 0 app
```

## Remove Google plus
```bash
pm uninstall -k --user 0 com.google.android.googlequicksearchbox

```

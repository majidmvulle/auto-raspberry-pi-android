# auto-raspberry-pi-android
Raspberry PI running Android 13 (Konstakang build) with some minor customizations on GPIOs to shutdown, start-up, etc

## Installation - Scripts

```shell
adb root
adb remount
adb push /path/to/script /vendor/etc/init.d/
```

OR

```shell
su
mount -o rw,remount /vendor
cp /path/to/script /vendor/etc/init.d/
chmod 755 /vendor/etc/init.d/<script-name>
chown root:shell /vendor/etc/init.d/<script-name>
```

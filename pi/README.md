
# Requirements

A bundle of tools are required, `dump` will precheck before working. Install these if missing.

```
check_bin "pv"        || exit 1
check_bin "fdisk"     || exit 1
check_bin "mount"     || exit 1
check_bin "parted"    || exit 1
check_bin "kpartx"    || exit 1
check_bin "mkfs.vfat" || exit 1
check_bin "mkfs.ext4" || exit 1
check_bin "losetup"   || exit 1
check_bin "blkid"     || exit 1
check_bin "dump"      || exit 1
check_bin "restore"   || exit 1
```

# dump

Backup `boot fs` and `root fs` from source device, to image file.

# setup/cleanup

`Setup` will setup local device from local image file, and mount to `./dst_root/` and `./dst_root/`.

`Cleanup` will undo what `Setup` does, umount directories and remove device.

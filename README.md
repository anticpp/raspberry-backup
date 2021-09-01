
# dump

Backup `boot fs` and `root fs` from source device, to image file.

# setup/cleanup

`Setup` will setup local device from local image file, and mount to `./dst_root/` and `./dst_root/`.

`Cleanup` will undo what `Setup` does, umount directories and remove device.

Overall, if you want to backup your pi system, there are 2 ways:

1. Dump the whole SDCard.

pros: It's easy

cons: You have to dumped the whole capacity size of SDCard, even used size is smaller. A 64GB image file will be dumped from a 64GB SDCard, even used size is 1GB, etc.

2. Dump filesystem of `boot` and `root` seperately.

pros: You can dump a smaller image file, which is actual the used size of your pi system.

cons: It's complicated. Because you have to handle partitions and dump boot/root filesystem seperately.

This repository have some toolkits to help doing the 2) way backup/restore flow.

# pi/

Using on raspberrypi.

# mac/

Using on mac.

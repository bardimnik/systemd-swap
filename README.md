systemd-swap
Simple script to auto create zram and swap file (through loop) devices and swapon it to system
Auto create ZRam devices (counts ZRam dev = CPU core counts)
It configurable in /etc/systemd-swap.conf
Source:
/etc/systemd/system/systemd-swap.service
/etc/systemd-swap.conf
/usr/lib/systemd/scripts/systemd-swap.sh

Using:
# systemctl enable systemd-swap
# systemctl start systemd-swap

TODO:
Dynamic increasing size of swap file;
Auto using direct method (without loop) to using swap files on friendly for swap file fs (ext(4,3,2),xfs & etc);
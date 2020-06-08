Raspberry Pi headless setup guide

# Ubuntu (32 or 64 bit)

1. Download image: https://ubuntu.com/download/raspberry-pi
2. Prepare sd-card: https://www.raspberrypi.org/documentation/installation/installing-images/linux.md
```sh
dd bs=4M if=image.img of=/dev/sdX status=progress conv=fsync
```
3. Shh is enabled by default
4. Setup wifi: https://ubuntu.com/tutorials/how-to-install-ubuntu-on-your-raspberry-pi#3-wifi-or-ethernet
5. Connect via ssh: user: ubuntu, password: ubuntu

# Raspbian (32 bit)

1. Download image: https://www.raspberrypi.org/downloads/raspberry-pi-os/
2. Prepare sd-card: https://www.raspberrypi.org/documentation/installation/installing-images/linux.md
```sh
dd bs=4M if=image.img of=/dev/sdX status=progress conv=fsync
```
3. Setup shh: https://www.raspberrypi.org/documentation/remote-access/ssh/README.md
4. Setup wifi: https://www.raspberrypi.org/documentation/configuration/wireless/headless.md
5. Connect via ssh: user: pi, password: raspberry

# Alternative connections

### Connect to PC through ethernet: 

- connect raspberry pi to laptop with Ethernet
- Go the edit connection setting.
- Navigate to ipv4 option. Select method : shared to other computer.
- Then open command prompt and type command >"cat /var/lib/misc/dnsmasq.leases". You will get raspberry pi Ip from that.
- then connect via ssh

Source: https://raspberrypi.stackexchange.com/questions/30144/connect-raspberry-pi-to-pc-ubuntu-with-ethernet

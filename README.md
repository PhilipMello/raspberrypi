# Raspberry Pi (Firmwares, OS, Configs)

## Configuration File Raspberry Pi
sudo nano /boot/firmware/config.txt

## Check Raspbrry Pi Temperature
vcgencmd measure_temp

## Change keyboard layout configuration
- XKBLAYOUT="us"
- XKBLAYOUT="pt"
```bash
sudo nano /etc/default/keyboard
```
OR
```bash
sudo nano sed -i 's/XKBLAYOUT="us"/XKBLAYOUT="pt"/'
```
Apply changes:
```bash
sudo setupcon
```

## Adjust the Fan Settings
- dtoverlay=rpi-poe  # Enables fan control
- dtparam=poe_fan_temp0=40000,poe_fan_temp0_hyst=2000  # Fan starts at 40°C, stops at 38°C
- dtparam=poe_fan_temp1=50000,poe_fan_temp1_hyst=2000  # 50% speed at 50°C
- dtparam=poe_fan_temp2=60000,poe_fan_temp2_hyst=2000  # 75% speed at 60°C
- dtparam=poe_fan_temp3=70000,poe_fan_temp3_hyst=2000  # 100% speed at 70°C

## How to remove snapd from ubuntu server
```bash
sudo systemctl stop snapd
sudo apt remove --purge snapd
sudo rm -rf /var/cache/snapd/
sudo rm -rf ~/snap
sudo apt autoremove
sudo reboot
snap --version
```

# zmk-config for charybdis (4x6)

### Remove old bluetooth device of Charybdis
0. bluetoothctl
remove [MAC:ADDR]

### Plug in the right side (main) / left side of the keyboard
1. cd /media/hustlenut/NICENANO

### Copy the reset file into the keyboard and wait for it to be done flashing
2. cp ~/Downloads/firmware/settings_reset-nice_nano_v2-zmk.uf2 .

### Copy the respective firmware file into the keyboard
3. cp ~/Downloads/firmware/charybdis_right-nice_nano_v2-zmk.uf2

### Do step 2 and 3 for both keyboards

### Trust the bluetooth device
4. bluetoothctl
trust [MAC:ADDR]

### Connect to the keyboard with bluetooth

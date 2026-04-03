![38702b81-94ea-4e85-bb2f-34790bd850b1~1](https://github.com/user-attachments/assets/5801fc41-0659-4f57-b26d-ceaa737fd155)
# SOLO_HUNTER **UPDATED** to -------->
# SOLO_HUNTER v1.0.1

SOLO_HUNTER is a DigiByte wallet display for ESP32 CYD / NerdMiner-style devices.

It shows:
- live DGB wallet balance
- estimated USD value
- a BLOCK FOUND popup when balance increases
- on-device settings for wallet address and screen flip

## Supported hardware
This version is built for:
- 1-USB NerdMiner V2 style device
- ILI9341 display

## Easiest install method
You do NOT need Arduino to use this version.

### What you need
- an ESP32 flashing tool
- the file: `SOLO_HUNTER_v1.0.1.bin`

### Flashing
Flash the firmware file at:

`0x0`

After flashing:
1. Power on the device
2. Connect to the WiFi network:
   `SOLO_HUNTER_SETUP`
3. Open the setup portal
4. Enter your WiFi info
5. Enter your DGB wallet address
6. Save settings

After setup, the device will connect to your WiFi and display your wallet info.

## Settings page
Once connected to WiFi, open the device IP address in your browser to:
- change wallet address
- flip screen rotation
- reopen WiFi setup if needed

## Files
- `SOLO_HUNTER_v1.0.1.bin` = prebuilt firmware for beginners
- `.ino` file = source code for advanced users

## Notes
- If USD value says `USD WAIT`, the wallet balance should still remain visible.
- This project was built to be simple for non-coders to flash and use.


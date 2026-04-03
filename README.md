![PXL_20260403_173620408~2](https://github.com/user-attachments/assets/fd775692-ddcc-4067-966c-988c059f310e)
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




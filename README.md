![PXL_20260403_173620408~2](https://github.com/user-attachments/assets/fd775692-ddcc-4067-966c-988c059f310e)
SOLO_HUNTER v1.0.2

SOLO_HUNTER is a DigiByte wallet display for ESP32 CYD / NerdMiner-style devices.

It shows:

live DGB wallet balance
estimated USD value
persistent BLOCK FOUND notification when balance increases
on-device settings for wallet address, screen flip, and alerts
🔧 What’s New in v1.0.2
Fixed USD WAIT text overflow (“AIT” bug)
Faster USD price loading
Displays device IP when no wallet is configured
BLOCK FOUND notifications now stay on screen until manually cleared
🧰 Supported Hardware

This version is built for:

1-USB NerdMiner V2 style device
ESP32 CYD (ESP32-2432S028)
ILI9341 display
⚡ Easiest Install Method

You do NOT need Arduino to use this version.

What you need
an ESP32 flashing tool (esptool, etc.)
the file: SOLO_HUNTER_v1.0.2_merged.bin
🚀 Flashing

Flash the firmware file at:

0x0

Example:

python -m esptool --chip esp32 --port COM7 --baud 921600 write_flash 0x0 SOLO_HUNTER_v1.0.2_merged.bin

(replace COM7 with your device port)

📶 First Setup

After flashing:

Power on the device
Connect to WiFi network:
SOLO_HUNTER_SETUP
Open the setup portal
Enter your WiFi credentials
Enter your DGB wallet address
Save settings

After setup, the device will connect to your WiFi and display your wallet info.

🌐 No Wallet Config Behavior

If no wallet is set, the screen will display:

SET WALLET <device IP>

Use that IP address in your browser to configure the device.

⚙️ Settings Page

Once connected to WiFi, open the device IP address in your browser to:

change wallet address
flip screen rotation
clear BLOCK FOUND notification
reopen WiFi setup if needed
📦 Files
SOLO_HUNTER_v1.0.2_merged.bin → prebuilt firmware (recommended)
.ino file → source code for advanced users
📝 Notes
USD value may briefly show USD WAIT, but balance will still display immediately
USD price now loads significantly faster than previous versions
BLOCK FOUND alerts will remain until cleared manually (so you don’t miss them)
💡 About This Project

This project was built to be simple, fast, and usable for home miners without requiring coding experience.

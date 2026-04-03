![PXL_20260403_173620408~2](https://github.com/user-attachments/assets/fd775692-ddcc-4067-966c-988c059f310e)
SOLO_HUNTER v1.0.2

SOLO_HUNTER is a DigiByte wallet display for ESP32 CYD / NerdMiner-style devices.

It provides a simple, real-time display of your wallet activity on a dedicated device.

✨ Features
Live DGB wallet balance
Estimated USD value
BLOCK FOUND notification when balance increases
Persistent alerts (must be manually cleared)
On-device settings (WiFi, wallet, screen flip)
🧰 Supported Hardware
Device Type	Screen	Firmware
ESP32 CYD / NerdMiner	ILI9341	SOLO_HUNTER_v1.0.2_merged.bin
ESP32 CYD / NerdMiner	ST7789	SOLO_HUNTER_v1.0.2_ST7789_merged.bin
⚠️ Important

You must use the correct firmware for your screen.

If you flash the wrong version, you may see:

blank screen
wrong colors
distorted or misaligned display

If that happens, just flash the other version.

🚀 Installation (ESP Flasher Tool)

You do NOT need Arduino.

What you need
ESP32 device
USB cable
Windows PC
ESP Flash Download Tool (or similar)
Correct .bin file
🔧 Flashing Steps
Open your ESP flashing tool
Select chip type:
ESP32
Select your COM port
Load the firmware file:
ILI9341 → SOLO_HUNTER_v1.0.2_merged.bin
ST7789 → SOLO_HUNTER_v1.0.2_ST7789_merged.bin
Set flash address:
0x0
Click Start / Flash

Wait for flashing to complete.

📶 First Setup

After flashing:

Power on the device
Connect to WiFi network:
SOLO_HUNTER_SETUP
Enter password:
solohunter
Open setup page
If it doesn’t open automatically, go to:
http://192.168.4.1
Enter:
your WiFi credentials
your DigiByte wallet address
Save settings

The device will connect and begin displaying your wallet data.

🌐 No Wallet Config

If no wallet is set, the device will display its IP address.

Open that IP in your browser to access settings.

⚙️ Settings Page

Open the device IP address in your browser to:

change wallet address
flip screen rotation
clear BLOCK FOUND notification
reopen WiFi setup
📝 Notes
BLOCK FOUND alerts stay on screen until manually cleared
USD price loads faster than previous versions
ILI9341 and ST7789 require different firmware files
📦 Files
SOLO_HUNTER_v1.0.2_merged.bin → ILI9341 firmware
SOLO_HUNTER_v1.0.2_ST7789_merged.bin → ST7789 firmware
.ino files → source code
💡 About

This project was built to be simple, fast, and usable for home miners without requiring coding experience.

🔜 Coming Next
ST7789 refinement
dual-screen auto support (future goal)
UI improvements

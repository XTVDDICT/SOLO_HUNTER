![PXL_20260403_173620408~2](https://github.com/user-attachments/assets/fd775692-ddcc-4067-966c-988c059f310e)
SOLO_HUNTER v1.0.2

SOLO_HUNTER is a DigiByte wallet display for ESP32 CYD / NerdMiner-style devices.

Features
live DGB wallet balance
estimated USD value
BLOCK FOUND notification when balance increases
on-device settings (wallet, WiFi, screen flip, alert clear)
Supported Hardware
✅ Currently Supported
ESP32 CYD / NerdMiner-style devices
ILI9341 display
🚧 Coming Soon
ST7789 display support (in progress)
Files
SOLO_HUNTER_v1.0.2_merged.bin → prebuilt firmware (ILI9341 only)
SOLO_HUNTER_v1_0_2.ino → source code
🚀 Installation (ESP Flasher Tool – Recommended)

You do NOT need Arduino.

What you need
ESP Flasher tool (ESP Flash Download Tool or similar)
SOLO_HUNTER_v1.0.2_merged.bin
Flashing Steps
Open the ESP Flasher tool
Select your COM port
Load the file:
SOLO_HUNTER_v1.0.2_merged.bin
Set the flash address to:
0x0
Click Start / Flash
After Flashing
Power on the device
Connect to WiFi network:
SOLO_HUNTER_SETUP
Enter password:
12345678
Open the setup portal (should open automatically)
If not, go to: 192.168.4.1
Enter your WiFi credentials
Enter your DGB wallet address
Save settings

The device will connect to your WiFi and begin displaying wallet data.

No Wallet Config

If no wallet is set, the device will display its IP address so you can open the settings page and configure it.

Settings Page

Open the device IP in your browser to:

change wallet address
flip screen rotation
clear BLOCK FOUND notification
reopen WiFi setup
Notes
BLOCK FOUND alerts stay on screen until manually cleared
USD price loads faster than previous versions
This release is ILI9341 only
ST7789 support coming soon

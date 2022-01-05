# X570-Aorus-Eite-WiFi-EFI
OpenCore 0.7.6 EFI\n

This EFI is partially functional:

MoBo: Gigabyte X570-Aorus Elite WiFi\n
CPU: Ryzen 7 3900X\n
GPU: Gigabyte AMD Radeon R580\n
Ethernet: Intel Integrated I211(MoBo)\n
Bluetooth: Integrated (MoBo)\n
WiFi: Intel Wi-Fi 802.11 a/b/g/n/ac\n
NVMe: Samsung 980Pro\n
RAM: Neo Forza 3600MHz\n

What works:
WiFi
iMessage/Facetime/AppleID
Audio
USB2 port personality (minus one port)
USB3 port personality (minus one port)
Sleep
Wired/RF keyboard/mouse wake from sleep
~6000 GB/s reads | ~1700 GB/s writes

What doesn't work:
Ethernet - sort of
Bluetooth

Issues: 
1) Ethernet works with manual IP, but breaks after wake from sleep
2) Long delay (5-10s) between boot log disappearing and login screen
3) No bluetooth
4) Haven't renamed usb controller -> USB devices don't show up in IORegistryExplorer

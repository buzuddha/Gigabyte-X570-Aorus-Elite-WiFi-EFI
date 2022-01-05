# X570-Aorus-Eite-WiFi-EFI  
OpenCore 0.7.6 EFI
Monterey 12.1 MacPro7,1

This EFI is partially functional:  

MoBo: Gigabyte X570-Aorus Elite WiFi  
CPU: Ryzen 7 3900X  
GPU: Gigabyte AMD Radeon R580  
Ethernet: Intel Integrated I211(MoBo)  
Bluetooth: Integrated (MoBo)  
WiFi: Intel Wi-Fi 802.11 a/b/g/n/ac  
NVMe: Samsung 980Pro  
RAM: Neo Forza 3600MHz  

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
3) No bluetooth (was getting incredibly slow boot times with IntelBluetoothInjector/IntelBluetoothFirmware - though that was prior to getting WiFi working)   
4) Haven't renamed usb controller -> USB devices don't show up in IORegistryExplorer  

I must thank the opencore community, AMD-OSX, EliteMacX86, Chris Titus Tech for his youtube video, and above all Dortania's guide  

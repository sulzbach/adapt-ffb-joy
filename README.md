# What is Adapt-FFB-Joy #

Adapt-FFB-Joy is an AVR microcontroller based device that looks like a joystick with advanced force feedback features in a Windows machine without need for installing any device drivers to PC.

This project contains the software for the AVR microcontroller as well as basic instructions for [building the hardware](https://github.com/tloimu/adapt-ffb-joy/blob/wiki/HowToBuild.md).

Currently, it allows connecting a Microsoft Sidewinder Force Feedback Pro (FFP) joystick (with a game port connector) to various MS Windows versions as a standard **USB joystick with force feedback** and **no need to install any device drivers**. The adapter also allows to solder a few additional trim pots to work e.g. as elevator trims, aileron trims and rudder pedals in your favorite simulator game.

For more information, see [Adapt-ffb-joy Wiki] (https://github.com/tloimu/adapt-ffb-joy/blob/wiki/README.md)

The firmware software project is configured to compile for ATmega32U4 with WinAVR-20100110 or newer version.

On MacOS:

```bash
| +-o LUFA Joystick wFFB@04100000  <class AppleUSBDevice, id 0x10000102b, registered, matched, active, busy 0 (47 ms), retain 19>
  |     {
  |       "sessionID" = 12748255553063
  |       "iManufacturer" = 1
  |       "bNumConfigurations" = 1
  |       "idProduct" = 8270
  |       "bcdDevice" = 1
  |       "Bus Power Available" = 500
  |       "USB Address" = 3
  |       "bMaxPacketSize0" = 8
  |       "iProduct" = 2
  |       "iSerialNumber" = 0
  |       "bDeviceClass" = 239
  |       "Built-In" = No
  |       "locationID" = 68157440
  |       "bDeviceSubClass" = 2
  |       "bcdUSB" = 272
  |       "USB Product Name" = "LUFA Joystick wFFB"
  |       "PortNum" = 1
  |       "non-removable" = "no"
  |       "IOCFPlugInTypes" = {"9dc7b780-9ec0-11d4-a54f-000a27052861"="IOUSBFamily.kext/Contents/PlugIns/IOUSBLib.bundle"}
  |       "bDeviceProtocol" = 1
  |       "IOUserClientClass" = "IOUSBDeviceUserClientV2"
  |       "IOPowerManagement" = {"DevicePowerState"=0,"CurrentPowerState"=4,"CapabilityFlags"=32768,"MaxPowerState"=4,"DriverPowerState"=4}
  |       "Device Speed" = 1
  |       "USB Vendor Name" = "Dean Camera"
  |       "idVendor" = 1003
  |       "IOGeneralInterest" = "IOCommand is not serializable"
  |       "IOClassNameOverride" = "IOUSBDevice"
  |     }
```

```bash
 | +-o LUFA Wheel wFFB@04100000  <class AppleUSBDevice, id 0x100001079, registered, matched, active, busy 0 (1224 ms), retain 19>
  |     {
  |       "sessionID" = 13019181753592
  |       "iManufacturer" = 1
  |       "bNumConfigurations" = 1
  |       "idProduct" = 8278
  |       "bcdDevice" = 1
  |       "Bus Power Available" = 500
  |       "USB Address" = 3
  |       "bMaxPacketSize0" = 8
  |       "iProduct" = 2
  |       "iSerialNumber" = 0
  |       "bDeviceClass" = 239
  |       "Built-In" = No
  |       "locationID" = 68157440
  |       "bDeviceSubClass" = 2
  |       "bcdUSB" = 272
  |       "USB Product Name" = "LUFA Wheel wFFB"
  |       "PortNum" = 1
  |       "non-removable" = "no"
  |       "IOCFPlugInTypes" = {"9dc7b780-9ec0-11d4-a54f-000a27052861"="IOUSBFamily.kext/Contents/PlugIns/IOUSBLib.bundle"}
  |       "bDeviceProtocol" = 1
  |       "IOUserClientClass" = "IOUSBDeviceUserClientV2"
  |       "IOPowerManagement" = {"DevicePowerState"=0,"CurrentPowerState"=3,"CapabilityFlags"=65536,"MaxPowerState"=4,"DriverPowerState"=3}
  |       "Device Speed" = 1
  |       "USB Vendor Name" = "Dean Camera"
  |       "idVendor" = 1003
  |       "IOGeneralInterest" = "IOCommand is not serializable"
  |       "IOClassNameOverride" = "IOUSBDevice"
  |     }
```
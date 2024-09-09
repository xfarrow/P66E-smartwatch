# How to communicate using the GATT protocol

1. Install `bluez`: `sudo apt-get install bluez`
2. Scan nearby devices using `sudo hcitool lescan` and obtain the MAC address of your smartwatch
3. Connect in interactive mode: `gatttool -b <MAC Address> -I`
4. Use GATT

**Example**

Type `primary` to list services

Output is: `attr handle: 0x0007, end grp handle: 0x000f uuid: 00001800-0000-1000-8000-00805f9b34fb` (GenericAccess service). 

To list its characteristics use `characteristics 0x0007 0x000f`

Output is: `handle: 0x0008, char properties: 0x02, char value handle: 0x0009, uuid: 00002a00-0000-1000-8000-00805f9b34fb`. `0x0008` is the address of the metadata, `0x02` states that it's a read-only property, `0x009` is the address of the actual data and the UUID `00002a00-0000-1000-8000-00805f9b34fb` specifies that's a DeviceName characteristic.

Read its content by `char-read-hnd 0x0009`

# Documentation
## Device's name
The device's name is exposed through the standard Bluetooth Generic Attribute Profile (GATT). This is the data read by any Bluetooth device scanning for nearby devices.

Service: ```GenericAccess``` (UUID: 00001800-0000-1000-8000-00805f9b34fb)

Characteristic: ```DeviceName``` (UUID: 00002a00-0000-1000-8000-00805f9b34fb)

Example output: ```50 36 36 45 28 49 44 2d 38 31 44 46 29 00``` which translates to "P66E(ID-81DF)"

## More
Other GATT characteristics seem to return unreadable data. Their purpose is unknown and hence the smartwatch does not follow the standard GATT specification. More analysis is needed.

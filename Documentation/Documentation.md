# Documentation
## Device's name
The device's name is exposed through the standard Bluetooth Generic Attribute Profile (GATT). This is the data read by any Bluetooth device scanning for nearby devices.

Service: ```GenericAccess```

Characteristic: ```DeviceName```

Example output: ```P66E(ID-81DF)``` (ASCII)

## More
Other GATT characteristics seem to return unreadable data. Their purpose is unknown and hence the smartwatch does not follow the standard GATT specification. More analysis is needed.

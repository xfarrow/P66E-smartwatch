# P66E
Reverse engineering a P66E smartwatch. This projects aims at writing its [technical documentation](https://github.com/xfarrow/P66E-smartwatch/blob/main/Documentation/Documentation.md) of operation and at developing a piece of software able to communicate with it without the need to use its official app.

Using the [Gadgetbridge's guide](https://codeberg.org/Freeyourgadget/Gadgetbridge/wiki/BT-Protocol-Reverse-Engineering).

### Other names
The P66E comes with different commercial names such as
- Ddidbi Smart Watch
- Sudugo P66E
- Poounur P66E
- Popglory P66

## What we know so far
Unfortunately this device does not adhere to the Bluetooth GATT specification. This will make the process of reverse engineering harder, as we need to sniff the traffic between the P66E and the companion app (Gloryfit).

# XRSP-Reversed
Reverse-engineering the Oculus Link / XRSP protocol.

# Format (TODO)
| Position | Size | Name                         |
|----------|------|------------------------------|
| 0x00     | Byte | XRSP Version (Latest = 0x18) |
| 0x01     | Byte | Topic                        |
| 0x02     | Byte | Length(?)                    |
| 0x03-?   | ?    | Topic Data(?)                |

# Topics
Topics are essentially IDs for various datatypes that XRSP has, they are 6-bits(?) in length and are masked to 0x3f (I think).

| ID   | Name                                                                               |
|------|------------------------------------------------------------------------------------|
| 0x01 | Device Descriptor (basically what type of device this is, e.g. Quest 2 or Quest 1) |

TODO: Everything.

# XRSP-Reversed
Reverse-engineering the Oculus Link / XRSP protocol.

# Format (TODO)
| Position | Name                         |
|----------|------------------------------|
| 0x00     | XRSP Version (Latest = 0x18) |
| 0x01     | Topic                        |
| 0x02     | Length(?)                    |

# Topics
Topics are essentially IDs for various datatypes that XRSP has, they are 6-bits(?) in length and are masked to 0x3f (I think).

| ID   | Name                                                                               |
|------|------------------------------------------------------------------------------------|
| 0x01 | Device Descriptor (basically what type of device this is, e.g. Quest 2 or Quest 1) |

TODO: Everything.

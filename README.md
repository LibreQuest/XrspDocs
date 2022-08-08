# XrspDocs
Reverse-engineering the Oculus Link / XRSP protocol.

# Format (TODO)
| Position | Size | Name                         |
|----------|------|------------------------------|
| 0x00     | Byte | XRSP Version (Latest = 0x18) |
| 0x01     | Byte | Topic                        |
| 0x02     | Byte | Length(?)                    |
| 0x03-?   | ?    | Topic Data(?)                |

# Topics
Topics are essentially IDs for various datatypes that XRSP has, they are 6-bits(?) in length and are masked to "0x3f" (I think). Certain topics are also encrypted, it is currently unknown as to how they are encrypted. When an XRSP device is connected, the first topic that the device sends is "0x01" and then the server may respond with the next appropriate topic.

| ID   | Name                                                                               | Encrypted |
|------|------------------------------------------------------------------------------------|-----------|
| 0x01 | Device Descriptor (basically what type of device this is, e.g. Quest 2 or Quest 1) | No        |

TODO: Everything.

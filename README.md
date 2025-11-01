# mcp2515_RXFn-RXMn_config
# RXFn 8bit
SIDH 11-3

SIDL 2-0

SID  0x85=SIDH: 0001 000 << 3 | SIDL: 1010 0000 >> 5

# RXMn 8bit
SIDH 11~3

SIDL 2~0

M1: SIDH: 1111 1111 << 3 | SIDL: 1110 0000 >> 5

M2: SIDH: 1111 1111 << 3 | SIDL: 0000 0000 >> 5

M3: SIDH: 1111 0000 << 3 | SIDL: 1110 0000 >> 5

|       | M1    | M2     | M3    |
| :-----| ----: | :----: |:----: |
| 0x85: 000 1000 0101  | true  | true   | true |
| 0x84: 000 1000 0101 | false | true |  false |
| 0x45: 000 0100 0101 | false | false |  true |

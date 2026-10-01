# Lab Inventory

| Label | Model | Serial | IOS | Image | DRAM | Flash | Config reg | Modules | Access |
|-------|-------|--------|-----|-------|------|-------|------------|---------|--------|
| R1 | CISCO2821 (V05) | FTX1338AH3N | 15.1(4)M10 IP Base K9 | c2800nm-ipbasek9-mz.151-4.M10.bin | 256 MB | 128 MB CF | 0x2102 | none | console open; enable password unknown |
| R2    |       |        |             |     |       |             |       |          |
| R3    |       |        |             |     |       |             |       |          |
| R4    |       |        |             |     |       |             |       |          |
| R5    |       |        |             |     |       |             |       |          |

## Notes
- R1 arrived as hostname `router7` with a saved config: Gi0/1 = 192.168.50.27, both interfaces shut down.
- Clock reads 2006; backup battery likely dead. NTP needed (Milestone 4).

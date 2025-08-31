# Endgame Trackball

Features:
1. Wireless (BLE) or wired (Type-C)
2. Twist-to-scroll as well as drag scroll (both high resolution)
3. Low profile and compact travel-friendly design
4. Guaranteed 250 Hz polling rate, up to 450 Hz when the sensors feel like it 
5. 8 buttons with magnetically attachable keycaps, 2 rotary encoders
6. Supported ball size: from 50.8 mm (2 inches) to 55 mm
7. Ball Transfer Units (BTU) or static bearings (hot swap with an adapter)
8. Up to 1500 mAh (102550 size) battery with 3 pin 1.0 mm connector
9. Fast charging (up to 15W) with QC and PD support
10. RGB underglow and vibration motor for feedback 

## Demo (more in [gallery](./GALLERY.md))

![20250728_060028](https://github.com/user-attachments/assets/f433f68a-cfca-4bec-8bcd-85bc274544f8)

## BOM

| Name                             | Qty | Note                                                                 |
|----------------------------------|-----|----------------------------------------------------------------------|
| Endgame Trackball PCB            | 1   |                                                                      |
| 3.7V battery                     | 1   | up to 102550, 3 pin 1.0 mm pitch, 1st pin negative                   |
| Trackball                        | 1   | 50.8 mm to 55 mm                                                     |
| PMW3610 and lens                 | 2   |                                                                      |
| Rotary encoder knob (wheel)      | 2   | SLA printed, Siraya Tech Blu biocompatible resin                     |
| Rotary encoder guide             | 1   | SLA printed part for assembly                                        |
| FPC, 150 mm                      | 2   | 0.5 mm pitch, 8 pin                                                  |
| FPC, 100 mm                      | 2   | 0.5 mm pitch, 8 pin                                                  |
| MR63ZZ bearing                   | 2   |                                                                      |
| BTU (optional)                   | 3   | BOSCH Rexroth (R0530108), Veichu VCN310 (with adapter)               |
| Static bearing (optional)        | 3   | 3 mm, Si3N4 (Silicon Nitride) recommended                            |
| Heat-set insert, M2\*3.5*2.5     | 16  | 3 more for static bearings adapters                                  |
| Magnet 4x2                       | 50  |                                                                      |
| M2 screw, 4 mm                   | 16  | ISO7380                                                              |
| M2 screw, 6 mm (optional)        | 3   | required for static bearings                                         |
| Rubber foot                      | 4   | 0.5 mm thickness                                                     |

## Roadmap

| Feature                       |       | Note |
|-------------------------------|-------|------|
| Wireless connectivity         | ✅    |      |
| Wired connectivity            | ✅    |      |
| High polling rate (USB/BLE)   | ✅    |      |
| Runtime rate limiting         | ⏳    | planned |
| Buttons configuration         | ✅    |      |
| Rotary encoders configuration | ⚠️    | not supported in ZMK Studio |
| Twist scroll                  | ✅    | tested only with high resolution scroll so far |
| Drag scroll                   | ✅    |      |
| Fast charging                 | ⚠️    | PD works, BC/QC planned |
| RGB                           | ✅    |      |
| Vibration                     | ⚠️    | only as feedback for sensitivity cycler so far |
| Sleep                         | ✅    |      |

## FAQ

Coming soon.

## Troubleshooting

Coming soon.

## Support

You can support me and the project here: [Ko-fi](https://ko-fi.com/efogdev).

# Endgame Trackball

Features:
1. Wireless (BLE) or wired (Type-C)
2. Twist-to-scroll as well as drag scroll (both high resolution)
3. Low profile and compact travel-friendly design
4. Guaranteed 250 Hz polling rate, up to 500 Hz when the sensors feel like it 
5. 8 buttons with magnetically attachable keycaps, 2 rotary encoders
6. Supported ball size: from 50 mm to 55 mm
7. Ball Transfer Units (BTU) or static bearings (hot swap with an adapter)
8. Up to 1500 mAh (102550 size) battery with 3 pin 1.0 mm connector
9. Fast charging (up to 15W) with PD support
10. RGB underglow and vibration motor for feedback 

## Demo (more in [gallery](./GALLERY.md), [the website](https://efog.tech/docs/colors) and [Discord](https://efog.tech/discord))

![20250728_060028](https://github.com/user-attachments/assets/f433f68a-cfca-4bec-8bcd-85bc274544f8)

## Default keymap
Available on the website: https://efog.tech/docs/keymap (or in the PDF directory)

#### Rotary encoders
- Default layer: left encoder — volume, right encoder — Ctrl+Tab / Ctrl+Shift+Tab
- Scroll layer: left — pointer sensitivity, right — twist scroll sensitivity
- Snipe layer: both — arrows (left/right)

## BOM

| Name                             | Qty | Note                                                                 |
|----------------------------------|-----|----------------------------------------------------------------------|
| Endgame Trackball PCB            | 1   |                                                                      |
| 3.7V battery                     | 1   | up to 102550, 3 pin 1.0 mm pitch, 1st pin negative                   |
| Trackball                        | 1   | 50.8 mm to 55 mm                                                     |
| PMW3610 and lens                 | 2   |                                                                      |
| Vibration motor                  | 1   | coin type                                                            |
| Rotary encoder knob (wheel)      | 2   | SLA printed, Siraya Tech Blu biocompatible resin                     |
| Rotary encoder guide             | 1   | SLA printed part for assembly                                        |
| FPC, 150 mm                      | 3   | 0.5 mm pitch, 8 pin                                                  |
| FPC, 100 mm                      | 1   | 0.5 mm pitch, 8 pin                                                  |
| MR63ZZ bearing                   | 2   |                                                                      |
| BTU (optional)                   | 3   | BOSCH Rexroth (R0530108), Veichu VCN310 (with adapter)               |
| Static bearing (optional)        | 3   | 3 mm, Si3N4                                                          |
| Heat-set insert, M2\*3.5*2.5     | 9   |                                                                      |
| Magnet 4x2                       | 36  |                                                                      |
| M2 screw, 4 mm                   | 20  | ISO7380                                                              |
| Rubber foot                      | 4   | 0.5 mm thickness                                                     |

## Roadmap

| Feature                       |       | Note |
|-------------------------------|-------|------|
| Wireless connectivity         | ✅    |      |
| Wired connectivity            | ✅    |      |
| High polling rate (USB/BLE)   | ✅    |      |
| Runtime rate limiting         | ✅    |      |
| Buttons configuration         | ✅    | with ZMK Studio |
| Wheels configuration          | ✅    | with ZMK Studio |
| Twist scroll                  | ✅    | tested only with high resolution scroll so far |
| Drag scroll                   | ✅    |      |
| Fast charging                 | ⏳    | PD works (with exceptions), BC/QC planned (driver required) |
| RGB                           | ⏳    | only simple effects, no layer or battery indication so far     |
| Vibration                     | ✅    |      |
| Sleep                         | ✅    |      |
| 2.4 GHz dongle (≤1000 Hz)     | ⏳    | in progress     |
| 2.4 GHz dongle (8000 Hz)      | ⏳    | planned     |

## FAQ
Please see [FAQ.md](./FAQ.md).

## Troubleshooting
Please see [firmware thoubleshooting](https://github.com/efogtech/endgame-trackball-firmware/?tab=readme-ov-file#troubleshooting).

## Support

You can support me and the project here: [Ko-fi](https://ko-fi.com/efogdev).

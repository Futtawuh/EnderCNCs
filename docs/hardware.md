# Hardware Overview

This guide covers the core hardware needed to convert your Ender 3 (or Ender 3 Pro) into a desktop CNC machine. Parts are broken into reused components, items to purchase, and optional upgrades. Wherever possible, the BOM is aligned with common Voron 3D printer parts to make sourcing easier for hobbyists.

## Reused Ender 3 Parts

* **Frame & Structural Components** – keep most of the original aluminum extrusions and screws.
* **Electronics** - Original V1 and V4 MCU's have been tested.
* **Motors & Wiring** – stepper motors, wiring harnesses, and couplers.
* **Limit switches** – reuse up to 3, but you’ll need at least 1 additional switch.
* **Belts & Bearings** – 2 belts can be reused; plan to buy extra. Use existing bearings.
* **Fasteners** – most M3, M4, and M5 nuts and bolts can be salvaged.

!!! Note
    Modifications such as cutting the top 2020 extrusion for the z-axis require careful measurement.

## Differences betwen Ender 3 printers

Before diving in there a few key differences between versions of Ender 3 3D printers and are worth noting. This may affect your decision if you are looking at models for this project.

* Ender 3 and Ender 3 pro are essentially the same for the CNC conversion, the most significant difference is the extrusion used for the gantry (the Y extrusion that the Bed rides on).
* The rest of Ender 3 models are not covered here as they have not been tested but are here for awareness, they may or may not be suitable.

![Ender 3 vs pro](images/ender-3-series.png)

### Differences

| Part                     | Ender 3  | Ender 3 Pro             | CNC Implication                                                 |
| ------------------------ | -------- | ----------------------- | --------------------------------------------------------------- |
| Y-axis plate Extrusion   | 2040     | 4040                    | Gantry needs a 300mm extrusion purchased if original Ender 3    |
| V-wheels / rollers       | Plastic  | Slightly higher quality | CNC conversion uses same wheels but alignment becomes critical. |
| Screws & T-nuts          | Standard | Some upgraded           | Reuse as much as possible; minor differences.                   |
| Electronics              | V1.1.x   | V4.2.x                  | The Pro version is a better MCU                                 |

!!! note
    There is a mod to utilize the 2040 v-slot 300m gantry extrusion on the non pro but we do not recommend it. We recommend buying 2x 2040 v-slot 300m extrusions for $12 and fabricating the 4040 that the pro comes with and is explained in the gantry section.

## Parts from Ender 3 

| Qty | Part Description        | Notes                             |
|-----|-------------------------|-----------------------------------|
| **Extrusions**                                                    |
| 1x  | 2020 v-slot Profile     | To be cut in half                 |
| 2x  | 4040 v-slot Profile     |                                   |
| 2x  | 2040 v-slot Profile     |                                   |
| 1x  | 4040 v-slot Profile     | Ender 3 Pro Only                  |
| **M5 Screws**                                                     |
| 10x | M5x30 button head       |                                   |
| 16x | M5x45 bolts             | From the frame (remove shims)     |
| 4x  | M5x8                    |                                   |
| 1x  | M5x65                   | Middle lower X axis wheel         |
| All | M5 nuts                 |                                   |
| **M4 Screws**                                                     |
| 2x  | M4x20                   |                                   |
| 2x  | M4x16                   |                                   |
| 2x  | M4x10                   | Includes 2x M4 t-nuts             |
| **M3 Screws**                                                     |
| 6x  | M3x10                   |                                   |
| 11x | M3x10                   | Additional needed                 |
| 4x  | M3x40                   |                                   |
| 12x | M3x6                    |                                   |
| **Bearings**                                                      |
| 2x  | 688 bearings            | If available                      |

!!! Note
    You can re-use 2 belt lengths from the Ender 3, but you still need one more ~350mm length. 

!!! Tip
    You can re-use 3 limit switches from the Ender 3, if you want to cut them off the PCB's but you'll still be missing 1, so you need to order AT LEAST 1 more, it is probably easier just to buy a new set if you go with this option. The recommendation is to go with the endstop mod.
    

## Parts to Purchase (BOM) Bill of Materials

| Qty | Part Description    | Specifications           | Notes                      |
|-----|---------------------|--------------------------|----------------------------|
| **Extrusion**                                                                     |
| 2x  | 2040 v-slot         | 300mm                    | Only for Original Ender    |
| **Motion Components**                                                             |
| 3x  | GT2 belts           | 350mm length, 6mm width  | Buy 3-5 meter roll         |
| 3x  | GT2 pulleys         | 20T, 6mm width, 5mm bore |                            |
| 2x  | MGN12H linear rails | 150mm length             | 1 carriage per rail        |
| 2x  | 608ZZ bearings      | 8x22x7mm                 | Or use 688 from Ender 3    |
| **Electronics**                                                                   |
| 4x  | D2F-L Microswitch   | Limit switch             | Get 10 pack / use original |
| **Fasteners**                                                                     |
| 20x | M3 T-nuts           | For 2020 extrusion       | Sliding or standard t-nuts |
| 40x | M5 T-nuts           | For 2020 extrusion       | Sliding or standard t-nuts |
| 10x | M5 locknuts         | Hex nuts                 |                            |
| 70x | M5x16 button head   |                          |                            |
| 22x | M3x10 screws        | Not countersunk          |                            |
| 12x | M3x8 SHCS           | Socket head cap screws   |                            |
| **Hardware**                                                                      |
| 30x | Heat set inserts    | M3x4x5mm                 | Voron spec                 |
| 4x  | M5 shims            | OD 10mm, ID 5mm, 1mm     | Washers                    |

## Optional Upgrades

| Qty | Part Description | Specifications               | Purpose                               |
|-----|------------------|------------------------------|---------------------------------------|
| 8x  | Aluminum spacers | 5mm ID x 8mm OD x 8mm length | Replaces printed Y axis wheel spacers |


---

## Self sourcing 

!!! warning
    If you can't find a reasonable priced Ender 3 you can self source the parts from the jungle store.

This is to give you an idea of the cost if you were to build your own classic Ender 3 printer. It does not include all the parts that came with the original Ender, it is just a ballpark figure for people interested. When buying it is cheaper to buy in quantity to save money so our example here is for two printers.

**Cost for profiles:**

- 2020 profiles - 330 + 345 = 675 mm [Amazon $18](https://www.amazon.com/Seekliny-Aluminum-Extrusion-V-Slotted-Accessories/dp/B0DY7D8B23) 2 extra
- 2040 profiles - 330 + 400 + 400 = 1,130 mm [Amazon $18](https://www.amazon.com/400mm-Aluminum-Extrusion-European-Standard/dp/B0DST7TW3Z) 0 extra so buy 2 $36
- 4040 profiles - 250 + 290 + 290 = 830 mm [Amazon $55 4x600mm](https://www.amazon.com/Aluminum-Extrusion-European-Standard-Anodized/dp/B09MYGZDW4)  cut to appropriate length enough for 2

**Two frames total = $109/2 or $55 each**

**Other essential parts**

- Power supply [Amazon $22](https://www.amazon.com/SHNITPWR-Switching-Converter-Transformer-Security/dp/B07TWW8Q73) x2
- 42-34 Motor [Amazon $27](https://www.amazon.com/YEJMKJ-Stepper-41-07oz%C2%B7-Bipolar-Printer/dp/B0FHHV9JZG) x2
- 42-40 Motor [Amazon $22](https://www.amazon.com/Printer-Stepper-42-40-Extruder-Creality/dp/B0CSW9KG8H) 1 each

**Total for 2 (frame/motor/power) = $229 (add 2x$50 electronics) or about $170 each**

---

## Ready to Proceed?

Once you have the required parts, continue to the next section to review required printed parts.

<p align="center">
  <a href="/EnderCNC/printed_parts" class="md-button md-button--primary">
    Continue to Printed Parts →
  </a>
</p>

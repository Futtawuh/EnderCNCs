# Ender 3 PRO based CNC Build manual (not finished)

### !! Note: This "guide" might contain errors with hardware parts, if you find any issue please let me know !!

## Things you'll need. 
- Ender 3 PRO (not the non pro version)
- M5 tap
- Ability to cut Alu extrusions to length.
- Hexdrives
- RaspberryPi or old laptop running linux/klipper. (if you want to use klipper)
- Dremel/Spindle of your choice (You might have to adjust the dremel clamps to fit yours)
- Printed pressfit pulley extraction tool (this can be tricky, but you can also cut the off if you want)

### Print settings I used: PLA+, 5 wall, 5 top, 5 bottom, 40% gyroid.

## Bearing Choice
### If you dont have 608Z use the F688Z from the Ender 3 Pro X axis tensioner. 
![bearing_choice](https://github.com/user-attachments/assets/d841fb1d-110e-4ea4-9d34-9ba2e50c555c)

## M3 Heatsets ( M3x5x4 "Voron spec") 

### X-Motor plate
![image](https://github.com/user-attachments/assets/7332b77a-6eb4-4d05-9346-cdc946e39018)

### Corner Brackets
![corner_heatsets](https://github.com/user-attachments/assets/06044989-acee-415d-8073-7125a64f05ce)

### XZ Carriage Plate
![XZ_gantry_heatsets](https://github.com/user-attachments/assets/4fba9685-d5d5-408a-81e0-5332c101e72b)

### Dremel Plate
![dremel_plate_heatset](https://github.com/user-attachments/assets/914e1b90-3d9a-4424-9e26-8e420fbec676)

### Z Carriage
![Z_carriage_heatsets](https://github.com/user-attachments/assets/64c9cadd-f4e9-4abc-87e2-47490f4da957)

### XY Joints 
![XY_joints_heatsets](https://github.com/user-attachments/assets/bd5b7e90-6996-4121-8462-ed7e13717325)

## M5 Locknuts - These should be pressfits!

### Z Carriage 
![pressfit m5 hexnuts](https://github.com/user-attachments/assets/0c3ac4f8-af64-4019-a32e-04f9a0526972)

### XZ Carriage Plate
![xz_plate_pressfit m5 hexnuts](https://github.com/user-attachments/assets/1a03e0ed-d0fd-46fe-8d61-cae9c9132e79)

## Blind Joints

### Front 
![blind joint front](https://github.com/user-attachments/assets/08630ece-b02c-4bb3-bf43-59ef3e6ea5a9)

### Back
* Should be offset by 20mm to gain more Y axis travel.
  
![blind joint back](https://github.com/user-attachments/assets/a60326e6-98f7-465b-b56b-e87a3059d8f2)

### What is this part? 
* This is the "X Endstop Buffer". It attaches to the X motor plate on the X endstop side to a heatinset.
* This "buffer" is needed if you are homing with the vacuum attachment or "splashguards" on to not collide in the Y extrusion.
* You will not need this attached if you are not using the vacuum attachment.
* M3x8/10 screw

![image](https://github.com/user-attachments/assets/dae67f85-132f-4a61-aa68-f116240c1711)
![image](https://github.com/user-attachments/assets/32621413-e2cf-435e-a9be-b557d48f16bb)




# The build! 

### DO NOT PRESS IN THE ENDSTOPS AT ANY POINT UNTILL YOU START WIRING! YOU MIGHT NOT GET THEM OUT AGAIN AS THEY ARE PRESSFITS. 

## Frame
| Qty  | Item           | Source  | Notes |
|------|----------------|---------|-------|
| 48pc | M5x16 BHSC     | BUY     |       |
| 4pc  | M5x40          | Ender3  |       |
| 4pc  | M5x8           | Ender3  |       |
| 4pc  | M5 1mm Shims   | BUY     |       |
| 52pc | M5 T-nuts      | BUY     |       |

* DO NOT PRESS IN THE ENDSTOPS YET.
* Assemble frame as shown, take note of blind joints and 20mm offset on the back extrusion and check for square.
  - I found it easier to get a square frame on a known flat surface by adding the XY joints after the frame is built. Its a bit tricky, but very doable.

![assable_frame](https://github.com/user-attachments/assets/e2e27689-e391-477f-b41b-ad53ba24886d)

## XY joints
| Qty  | Item                                   | Source | Notes                                                  |
|------|----------------------------------------|--------|--------------------------------------------------------|
| 8pc  | M5x45 SHSC                             | Ender3 | Remove the shims from these                           |
| 8pc  | M3x10                                   | BUY    |                                                        |
| 8pc  | 8mm Spacer (Printed or 5mm bore Alu)   | BUY    | Do not use the aluminum spacers from the Ender3 here  |

* DO NOT PRESS IN THE ENDSTOP YET.
* Loosely attach the 20T pylleys.
* Assemble XY joints as shown WITHOUT the endstop.

![image](https://github.com/user-attachments/assets/af060d03-84d5-4548-8cf6-c7b0d1be8810)


## Mount XY joints to the frame. 
| Qty  | Item         | Source         | Notes |
|------|--------------|----------------|-------|
| 8pc  | V-Wheels     | Ender3         |       |
| 8pc  | M5 Locknuts  | Ender3 or BUY  |       |

* DO NOT PRESS IN THE ENDSTOP YET.
  - I slid the xy joint on while the frame was built.
  - Put on the 2 bottom wheels and loosely add M5 nut to them.
  - Place the bottom wheels in the V slot, hold it at a slight angle.
  - Add the 2 top wheels to the Vslot and angle up the XY joint with a slight wiggle the top screws should pop in the wheels.
  - Bit tricky but doable. Or if you want to just take of the 2040 from the frame and slide them on. Might need to re-square the frame though.
* After mounting both XY joints, doublecheck the measurement between the X extrusion mounting points before cutting the X extrusion.
* Ender 3 frames might not be 100% the same. so yours might be +- from 300mm.
* After cutting the X extrusion to size you need to tap 4 new m5 threads on the cut side.

![x_beam](https://github.com/user-attachments/assets/ccb7c652-776b-4105-b073-0b292099cf61)

## Assemble X+Z Carriage
| Qty   | Item                    | Source   | Notes                        |
|-------|-------------------------|----------|------------------------------|
| 4pc   | M3x8 BHSC               | Ender3   |                              |
| 2pc   | M3x10                   | BUY      |                              |
| 10pc  | M5x16 BHSC              | BUY      |                              |
| 2pc   | M5x8 BHSC               | Ender3   |                              |
| 4pc   | M3x40                   | Ender3   |                              |
| 4pc   | M5x45 SHCH              | Ender3   | Remove the shims             |
| 1pc   | M5x65 BHSC              | BUY      |                              |
| 12pc  | M3x8 SHSC               | BUY      |                              |
| 2pc   | M3x16 BHSC              | Ender3   |                              |
| 9pc   | Alu Spacers             | Ender3   |                              |
| 1pc   | 28.35mm Printed Spacer  | Printed  |                              |
| 5pc   | V-wheels                | Ender3   |                              |
| 4pc   | 32.60 mm spacer         | Printed  |                              |
| 8pc   | M3x10 BHSC              | Ender3   |                              |

* DO NOT PRESS IN THE ENDSTOP YET.
* Cut Ender3 2020 extrusions to 150mm x2 pieces.
* Tap m5 threads in both ends of the 150mm 2020 extrusions.
* Press in bearings if you didnt already.
* Loosely attach the coupler to the Z motor.
* Loosely attach the 20T pulley to the X motor. 
* Attach both Z and X motors to their plates before continuing.
* Attach the 2020 extrusions as square and paralell as you can.
* Mount the X motor carriage to the ZX carriage with the wheels and spacers.
  - This can be a bit tricky, but doable after picking up the wheels and spacers from the floor a few times, sorry.
  - NOTE! Alu spacers from the Ender 3 are 8.35mm long, if you use 8mm long spacers from another source please use this [add part link here] printed spacer part for the lower middle wheel.
* Attach the Z bottom bearing plate and Z motor plate.
* Attach the MGN12 rails with the MGN12H carriages to the 2020 extrusions. (use a printed MGN12->2020 tool to get good alignment on the rails. Printables, Thingiverse etc)
  - NOTE! If you cut the 2020 a bit shorter than 150mm or the rails you ordered/cut are over 150mm dont worry, in the Z motor plate there are cutouts for the MGN rails to slide into if they are too long (max 4mm clearance)
* Attach the Z leadscrew nut to the Z carriage.
* Mount the Z carriage to the MGN12H carriages. - After mounting the Z carrige to the rails, slide it up and down to check for any binding in the rails, adjust rails if needed.
* Cut leadscrew to size. ~180mm but doublecheck with your setup. it should just about poke out of the lower Z bearing.  
* Screw in the leadscrew from the bottom bearing all the way to the Z motor coupler and secure it.
* Slide the assembly on the X extrusion that was cut to size. 

![image](https://github.com/user-attachments/assets/73a1652d-c0c2-4bb7-a2be-acec6fe921a0)
![image](https://github.com/user-attachments/assets/77d2ba43-ecc7-4f77-92b8-ad5840bc0d95)
![image](https://github.com/user-attachments/assets/81e4dd24-6af0-45d9-aec4-4afe465f2943)
![image](https://github.com/user-attachments/assets/1d12b738-2ca4-4740-9579-ff64bf323fd3)

## Attach the X+Z assembly to the XY joint.
| Qty  | Item         | Source  | Notes |
|------|--------------|---------|-------|
| 8pc  | M5x30 BHSC   | Ender3  |       |
| 4pc  | M5x16 BHSC   | BUY     |       |

![image](https://github.com/user-attachments/assets/5dcf89d9-cb52-42a5-8f56-694e93f29057)

## Run the belts
| Qty  | Item                      | Source  | Notes                                      |
|------|---------------------------|---------|--------------------------------------------|
| 3pc  | ~500mm GT2 6mm Belt       | BUY     | Control measure before cutting to length!! |
| 12pc | M3x10                     | BUY     | Migth be some spares from the Ender3       |
| 6pc  | Printed Belt Clamp        | Printed |                                            |

![image](https://github.com/user-attachments/assets/deb2774b-ea59-430a-a367-10d460285eb0)



# TO BE CONTINUED




# Wiring and Electronics

This chapter covers connecting limit switches, wiring the motors, and PSU setup.

---

## 1. Parts Required

| Qty | Item             | Source | Notes |
|-----|-----------------|--------|-------|
| 4pc | Limit Switches  | Buy    | Endstops for X/Y/Z |
| Wires | As needed     | Buy    | JST connectors optional |
| 1pc | Electronics Enclosure | Buy/Print | Fits Raspberry Pi / SKR board / SSR |
| PSU | Power Supply    | Buy    | Ensure safe handling |

---

## 2. Limit Switch Installation

1. Solder wires to all 4 limit switches.  
2. Insert switches into the press-fit slots in the frame.  
3. Test that switches sit securely:
   - If too tight → lightly sand faces.  
   - If too loose → add shims or a small amount of hot glue.  
4. Leave switches **unpressed** until the frame and carriage are fully installed.

![Limit Switch Wiring](images/471681334-3da706a2-3e1c-42b8-87ce-5e7f920d97a9.png)

---

## 3. Wire Management

1. Use zip-tie mounts for clean wire routing.  
2. Keep wires away from moving parts.  
3. Route motor, limit switch, and spindle wires neatly to the electronics enclosure.

![Zip-Tie Mounts](images/471683901-9707564c-00c8-45d0-8bc4-fbd0206f12f6.jpg)

---

## 4. Electronics Enclosure

1. Choose enclosure based on your board (Raspberry Pi, SKR Pico, 4.2.2, 4.2.7).  
2. Modify enclosure if necessary to fit additional components like SSR.  
3. PSU installation:
   - Only connect once wiring is fully complete.  
   - Practice safety and follow electrical guidelines.

![Electronics Enclosure](images/471685321-56185c27-e378-4418-afa9-d0d2b21476d9.png)

![Electronics Enclosure](images/471685419-116521b7-7949-4bc5-a8b3-a1c03da9da04.png)

---

### Warnings

!!! warning
    Do not power the machine before completing wiring and verifying all connections.

!!! tip
    Use an old laptop running Klipper as an alternative to a Raspberry Pi if needed.

---

## Ready to Proceed?

You have now completed the wiring and ready to move on to the **Firmware Setup**.

<p align="center">
  <a href="/EnderCNC/firmware" class="md-button md-button--primary">
    Continue to Firmware →
  </a>
</p>
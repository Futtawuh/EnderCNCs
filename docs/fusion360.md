# Fusion 360 Klipperized post processor

Transform your Fusion 360 CAM workflow into a CNC-ready G-code workflow compatible with Klipper. This guide shows how to install and use the **Klipperized post processor** created for MPCNC and similar machines.

## Credits

Post processor by [Zergie/mpcnc_post_processor](https://github.com/Zergie/mpcnc_post_processor)– thanks for making Klipper integration possible!

## Installation

1. **Download the Post Processor**
   Download the `.cps` file from the GitHub repository linked above.

2. **Open Fusion 360**
   Navigate to the **Manufacture** workspace.

3. **Import the Post Processor**

   * Click **Post Process** in the toolbar.
   * Click the **folder icon** to select a post from the library.
   * Click **Import**.
   * Browse to your downloaded `.cps` file and click **Select**.

4. **Confirmation**
   Once imported, your post processor will appear in the list of available posts.

   <img alt="image" src="https://github.com/user-attachments/assets/c243b043-7aa4-4c08-ac71-b8347e3aa145" />

---

### Usage Notes

* **Do NOT select "upload and run"**
        This will immediately start your CNC job — risky if your setup isn’t ready.
* **Avoid setting G1 moves to G0 rapids at first**
        Travel moves will become extremely fast. Familiarize yourself with your machine before enabling.

   <img alt="image" src="https://github.com/user-attachments/assets/a0539942-e08f-40a8-9d20-c747a97e7170" />

 * Double-check toolpaths and clearance heights before running a job.

 * Always simulate in Fusion 360 first to prevent collisions.

---

## Recommended Workflow

1. Prepare your 3D model or 2D sketch.
2. Generate toolpaths using **2.5D or 3D milling operations**.
3. Select the **Klipperized post processor** for your CNC machine.
4. Export the G-code.
5. Load into your Klipper interface (e.g., Mainsail, Fluidd) and test with small movements first.

---

### Fusion360 Video Tutorial

[![Watch the video](https://img.youtube.com/vi/WxLeKf4OOfY/0.jpg)](https://www.youtube.com/watch?v=WxLeKf4OOfY)
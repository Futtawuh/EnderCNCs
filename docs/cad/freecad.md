# FreeCAD Overview

FreeCAD is a free, open-source parametric CAD software that lets you create and modify 3D models with precision. For the Ender 3 CNC project, FreeCAD is used to design custom parts, adjust dimensions for your frame, and generate models for 3D printing.

Whether you’re resizing a carriage plate, designing a clamp, or checking fitment, FreeCAD provides the flexibility to make your CNC build repeatable and accurate.

---

## Why FreeCAD?

* **Parametric Design:** Modify any dimension or feature without starting over.
* **Community Driven:** Active development and many tutorials.
* **Cross-Platform:** Runs on Linux, Windows, and macOS.
* **File Export Options:** Supports STEP, STL, DXF, and more — ideal for CNC and 3D printing workflows.

---

## Recommended Workflows

### 1. Adjust Existing Parts

Many Ender3CNC components are already designed in FreeCAD. You can open the `.FCStd` files and tweak dimensions:

* Carriage spacing
* Clamp thickness
* Pulley clearance
* Mounting hole positions

**Tip:** Always save a backup of the original before making changes.

---

### 2. Create Custom Parts

Need a new part for your CNC? FreeCAD lets you:

1. Sketch 2D geometry on a plane.
2. Extrude, pad, or cut features to create a 3D model.
3. Add mounting holes, fillets, or chamfers for strength and fit.
4. Export to `.STL` for 3D printing or `.STEP` for CNC machining.

---

### 3. Verify Fit and Assembly

Use FreeCAD’s **Assembly Workbench** or simply check parts visually:

* Ensure rails and carriages align.
* Confirm belt paths are unobstructed.
* Check that the Z probe or endstops have proper clearance.

---

## Recommended Settings for Ender3CNC Parts

* Units: **Millimeters**
* Snap increments: **0.1 mm** for fine adjustments
* Export resolution: High for smooth 3D printing surfaces

---

### FreeCAD Video Tutorial

If you add the mkdocs-video plugin, you can embed a demo video of adjusting parts:

[![FreeCAD CAM Tutorial](https://img.youtube.com/vi/0VAIXvHTKVY/0.jpg)](https://www.youtube.com/watch?v=0VAIXvHTKVY)

---

## Resources

* [FreeCAD Official Website](https://www.freecadweb.org)
* [FreeCAD Forum](https://forum.freecadweb.org)
* [FreeCAD Tutorials on YouTube](https://www.youtube.com/results?search_query=freecad+tutorial)

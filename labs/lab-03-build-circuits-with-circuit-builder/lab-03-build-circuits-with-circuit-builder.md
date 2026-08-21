# Lab 3 — Build Circuits with Circuit Builder

**Course:** Technical Drawing with AutoCAD Electrical (TGS-2023037466)  ·  **Topic 02:** Analysing Technical Drawings
**Maps to:** A4 — analyse drawings to determine construction needs; assemble standard motor-control circuits

## Goal

Use Circuit Builder to insert a three-phase motor-control circuit built dynamically from your selections, then save a frequently used circuit and re-insert it from the icon menu.

## What you'll build

A schematic sheet containing a Circuit Builder motor circuit plus a saved, reusable circuit block.

**Tools:** Circuit Builder · Icon Menu · Schematic components · Saved circuits

![Lab 3 workflow](workflow.png)

## Starter files (in this folder)

- `2-0_Blank.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `autodesk-electrical-sample-project/` — AutoCAD Electrical multiwire/circuit sample project (wddemo.wdp) (provided in the controlled course-delivery package; intentionally omitted from the public GitHub repository)

> **Compatibility safeguard:** Copy the complete package before opening it. These project files may contain legacy AutoCAD Electrical 2015 library paths. If prompted, allow the current Electrical toolset to update the copy, then remap missing NFPA/IEC or panel-library paths to the equivalent libraries installed with your current release. Never overwrite the supplied package.

## Step-by-step

1. Copy the supplied sample-project folder to your Lab 3 working area, open `wddemo.wdp`, and use DEMO02 plus DEMO10/DEMO11 as completed circuit references. Work only in your copy.

   ```
   AEPROJECT → Open Project → wddemo.wdp
   ```

2. Add 2-0_Blank.dwg to your TRAINING project and insert a ladder to carry the circuit.

   ```
   AELADDER
   ```

3. Launch Circuit Builder from the Schematic tab and pick a 3-phase motor circuit from the tree.

   ```
   AECIRCBUILDER
   ```

4. Step through the Circuit Configuration dialog — select the disconnect, protection and control options; the circuit is built dynamically from your selections.

   ```
   Circuit Builder → Configure → Insert
   ```

5. Insert a push button and a selector switch from the Icon Menu to complete the control rung.

   ```
   AECOMPONENT  (Icon Menu)
   ```

6. Select the finished circuit and save it with Save Circuit to Icon Menu for reuse.

   ```
   Schematic → Circuit Clipboard → Save Circuit
   ```

7. Insert the saved circuit onto a clear area of the sheet and watch tags update to stay unique.

   ```
   Icon Menu → Saved Circuits
   ```


## Test it

The motor circuit sits on the ladder with unique component tags (M1, PB1 …), and your saved circuit re-inserts with automatically retagged components — construction needs are met without redrawing.

---
*© 2026 Tertiary Infotech Academy Pte Ltd (UEN: 201200696W) · Technical Drawing with AutoCAD Electrical · Version v6.1*
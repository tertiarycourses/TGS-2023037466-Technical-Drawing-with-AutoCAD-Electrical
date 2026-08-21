# Lab 1 — Set Up a New AutoCAD Electrical Drawing

**Course:** Technical Drawing with AutoCAD Electrical (TGS-2023037466)  ·  **Topic 01:** Introduction to Technical Drawing Using AutoCAD Electrical
**Maps to:** A1 — devise metrics and guidelines for technical drawing production (template, workspace, limits, units)

## Goal

Create a new drawing from the ACADISO template, then set the workspace, drawing limits and units — the production metrics every drawing in your organisation should start from.

## What you'll build

A correctly configured metric drawing sheet, saved as a reusable baseline for the rest of the course.

**Tools:** AutoCAD Electrical · ACADISO template · Status bar · Grid & Snap

![Lab 1 workflow](workflow.png)

## Starter files (in this folder)

- `1-0_Blank.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `DraftingSettings.dwg`  (source: [PacktPublishing/Mastering-AutoCAD](https://github.com/PacktPublishing/Mastering-AutoCAD))

## Step-by-step

1. Start AutoCAD Electrical and create a new drawing from the ACADISO template (New → acadiso.dwt).

   ```
   NEW  →  acadiso.dwt
   ```

2. Set the Electrical workspace from the Workspace Switching control on the status bar.

   ```
   WSCURRENT  →  Electrical
   ```

3. Set the drawing limits to an A3 metric sheet (0,0 to 420,297) and Zoom All to see the full sheet.

   ```
   LIMITS 0,0 420,297   then   ZOOM All
   ```

4. Set the units to decimal millimetres with 0 precision (Format → Units).

   ```
   UNITS  →  Decimal · 0
   ```

5. Turn on Grid (F7) and Snap (F9) from the status bar and open DraftingSettings.dwg to compare a pre-configured sheet.

   ```
   GRID 10   ·   SNAP 10
   ```

6. Save the drawing as MyBaseline.dwg — this is your production guideline drawing.

   ```
   SAVEAS MyBaseline.dwg
   ```


## Test it

ZOOM All shows the full 420×297 sheet, the crosshair snaps in 10 mm increments, and STATUS reports decimal units — your baseline metrics are in force.

---
*© 2026 Tertiary Infotech Academy Pte Ltd (UEN: 201200696W) · Technical Drawing with AutoCAD Electrical · Version v6.1*
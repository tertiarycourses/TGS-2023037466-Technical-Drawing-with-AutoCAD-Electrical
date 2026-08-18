# Lab 2 — Create a Project with Project Manager

**Course:** Technical Drawing with AutoCAD Electrical (TGS-2023037466)  ·  **Topic 01:** Introduction to Technical Drawing Using AutoCAD Electrical
**Maps to:** A1, A2 — standardise production with a project; solve multi-drawing organisation problems

## Goal

AutoCAD Electrical is project-based: a .wdp project groups interrelated drawings so project-wide functions can retag and renumber. Create a project, add the supplied electrical plan drawings, and reorder them.

## What you'll build

A working .wdp project containing the supplied power and lighting plan drawings plus a title block, in the correct sheet order.

**Tools:** Project Manager · .wdp project file · Power_Plan / Lighting_Plan DWGs

![Lab 2 workflow](workflow.png)

## Starter files (in this folder)

- `10-2_Power_Plan.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `10-2_Lighting_Plan.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `Title_Block.dwg`  (source: [DCS-training/AutocadSelfLearn](https://github.com/DCS-training/AutocadSelfLearn))

## Step-by-step

1. Open Project Manager from the Project tab (it is a palette — dock it on the left).

   ```
   AEPROJECT
   ```

2. Create a new project named TRAINING — the .wdp file stores the project description and settings.

   ```
   Project Manager → New Project → TRAINING
   ```

3. Review the Project Properties: library standard (IEC/IEEE/NFPA), component tag format and cross-reference style.

   ```
   Right-click project → Properties
   ```

4. Add the supplied drawings 10-2_Power_Plan.dwg and 10-2_Lighting_Plan.dwg to the project.

   ```
   Right-click project → Add Drawings
   ```

5. Drag and drop the drawings inside Project Manager so the power plan is sheet 1, and add Title_Block.dwg as reference-only.

   ```
   Drag to reorder · Properties → Reference Only
   ```

6. Make TRAINING the active project and open a drawing from the project list by double-clicking it.

   ```
   Right-click → Activate
   ```


## Test it

Project Manager shows TRAINING in bold (active) with the drawings in your chosen order, and the .wdp file exists in the project folder — project-wide functions now see every sheet.

---
*© 2026 Tertiary Infotech Academy Pte Ltd (UEN: 201200696W) · Technical Drawing with AutoCAD Electrical · Version v6.0*
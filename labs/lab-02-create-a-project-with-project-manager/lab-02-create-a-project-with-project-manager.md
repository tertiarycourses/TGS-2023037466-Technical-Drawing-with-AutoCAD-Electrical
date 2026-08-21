# Lab 2 — Create a Project with Project Manager

**Course:** Technical Drawing with AutoCAD Electrical (TGS-2023037466)  ·  **Topic 01:** Introduction to Technical Drawing Using AutoCAD Electrical
**Maps to:** A1, A2 — standardise production with a project; solve multi-drawing organisation problems

## Goal

AutoCAD Electrical is project-based: a .wdp project groups interrelated schematic and panel drawings so project-wide functions can retag, renumber, cross-reference and report. Inspect the supplied AutoCAD Electrical sample project, then create a safe working copy for the connected labs.

## What you'll build

A verified working copy of an AutoCAD Electrical .wdp project, with its schematic and panel sheets in the correct order and current library paths resolved.

**Tools:** Project Manager · .wdp/.aepx project files · linked schematic and panel DWGs

![Lab 2 workflow](workflow.png)

## Starter files (in this folder)

- `10-2_Power_Plan.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `10-2_Lighting_Plan.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `Title_Block.dwg`  (source: [DCS-training/AutocadSelfLearn](https://github.com/DCS-training/AutocadSelfLearn))
- `autodesk-electrical-sample-project/` — AutoCAD Electrical sample project (wddemo.wdp with linked DEMO drawings) (provided in the controlled course-delivery package; intentionally omitted from the public GitHub repository)

> **Compatibility safeguard:** Copy the complete package before opening it. These project files may contain legacy AutoCAD Electrical 2015 library paths. If prompted, allow the current Electrical toolset to update the copy, then remap missing NFPA/IEC or panel-library paths to the equivalent libraries installed with your current release. Never overwrite the supplied package.

## Step-by-step

1. Copy the entire `autodesk-electrical-sample-project` folder to a new working folder named `TRAINING_PROJECT`; keep the supplied folder unchanged so it can be restored.

   ```
   File Explorer → Copy folder → TRAINING_PROJECT
   ```

2. Open Project Manager, select Open Project, and open `TRAINING_PROJECT\wddemo.wdp`. If prompted, allow AutoCAD Electrical to update the project/drawing format.

   ```
   AEPROJECT → Open Project → wddemo.wdp
   ```

3. Review Project Properties: schematic library standard, component tags, wire-number format and cross-reference style. If a legacy `Acade 2015` library path is reported, map it to the equivalent library installed with the current release.

   ```
   Right-click project → Properties → Project Settings
   ```

4. Expand the project and classify DEMO01–DEMO07 as schematic sheets and DEMO08–DEMO09 as panel sheets; confirm every listed drawing opens without a missing-file warning.

   ```
   Project Manager → expand project → open each drawing
   ```

5. Create a new project named TRAINING in the working folder and copy settings from `wddemo.wdp`; add the supplied power and lighting plan drawings for comparison.

   ```
   New Project → TRAINING.wdp → Copy Settings from Project
   ```

6. Reorder the drawings, set `Title_Block.dwg` as reference-only, activate TRAINING, and save a project copy before continuing to Lab 3.

   ```
   Drag to reorder · Properties → Reference Only · Activate
   ```


## Test it

Project Manager shows TRAINING in bold, every sample-project drawing resolves from the working folder, no unresolved legacy library path remains, and the original supplied package is unchanged.

---
*© 2026 Tertiary Infotech Academy Pte Ltd (UEN: 201200696W) · Technical Drawing with AutoCAD Electrical · Version v6.1*
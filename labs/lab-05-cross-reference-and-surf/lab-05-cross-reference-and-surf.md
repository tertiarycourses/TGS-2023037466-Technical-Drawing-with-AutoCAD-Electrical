# Lab 5 — Cross-Reference and Surf a Drawing Set

**Course:** Technical Drawing with AutoCAD Electrical (TGS-2023037466)  ·  **Topic 02:** Analysing Technical Drawings
**Maps to:** A3, A4 — review a multi-sheet set for accuracy with cross-references, Surfer and signal arrows

## Goal

Link a parent coil to its child contacts, break a wire across sheets with source/destination signal arrows, then audit the set with Surfer and Mark/Verify — how a checker reviews a real drawing set.

## What you'll build

A cross-referenced two-sheet circuit you can navigate with Surfer, plus a Mark/Verify change report.

**Tools:** Cross-referencing · Signal Arrows · Surfer · Mark/Verify · Reference DWG

![Lab 5 workflow](workflow.png)

## Starter files (in this folder)

- `10-1_Working_with_References.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `10-2_HVAC_Plan.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))

## Step-by-step

1. Insert a relay coil (parent) on sheet 1 and a NO contact (child) on sheet 2 of your project; assign the child to the parent in the Insert/Edit Child dialog.

   ```
   AECOMPONENT → coil / contact
   ```

2. Update cross-references and read the parent's contact grid — it reports where every child lives.

   ```
   AEXREF
   ```

3. Break a wire network across the two sheets with a Source arrow (assign a code) and a matching Destination arrow.

   ```
   AESOURCE  ·  AEDEST
   ```

4. Right-click the coil and Surf: jump between the parent, children and signal arrows from the Surf list.

   ```
   AESURF
   ```

5. Mark the project (Mark/Verify), move one component, then run Verify to get the change report.

   ```
   AEMARKVERIFY
   ```

6. Open the supplied reference drawings and identify which sheets are reference-only in Project Manager.

   ```
   OPEN 10-1_Working_with_References.dwg
   ```


## Test it

Surfer jumps coil → contact → signal arrow across sheets without manual searching, and the Verify report lists exactly the one component you moved — the set is auditable for accuracy.

---
*© 2026 Tertiary Infotech Academy Pte Ltd (UEN: 201200696W) · Technical Drawing with AutoCAD Electrical · Version v6.0*
# Lab 8 — Plot and Publish the Project to PDF

**Course:** Technical Drawing with AutoCAD Electrical (TGS-2023037466)  ·  **Topic 03:** Reviewing Technical Drawings for Strategic Relevance and Standard Compliance
**Maps to:** A6 — output the drawing set to submission standards (A3 sheets, hyperlinked multi-sheet PDF)

## Goal

Attach an external reference, then plot a drawing to an A3 PDF and publish the whole project to a single multi-sheet PDF with hyperlinks — the final conformance step before submission.

## What you'll build

An A3 PDF plot of one sheet and a hyperlinked multi-sheet PDF of the whole project.

**Tools:** External References · Plot · Publish · Multi-sheet PDF · Layout tabs DWG

![Lab 8 workflow](workflow.png)

## Starter files (in this folder)

- `1-12_Using_Layout_Tabs.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `New_Office_Layout.dwg`  (source: [PacktPublishing/Mastering-AutoCAD](https://github.com/PacktPublishing/Mastering-AutoCAD))
- `autodesk-electrical-sample-project/` — AutoCAD Electrical multi-sheet sample project with title-block data (wddemo.wdp) (provided in the controlled course-delivery package; intentionally omitted from the public GitHub repository)

> **Compatibility safeguard:** Copy the complete package before opening it. These project files may contain legacy AutoCAD Electrical 2015 library paths. If prompted, allow the current Electrical toolset to update the copy, then remap missing NFPA/IEC or panel-library paths to the equivalent libraries installed with your current release. Never overwrite the supplied package.

## Step-by-step

1. Open a working copy of the supplied `wddemo.wdp`, confirm all nine sheets and title-block data resolve, and use that project for the multi-sheet publish check.

   ```
   AEPROJECT → Open Project → wddemo.wdp
   ```

2. Open the External References palette and attach a DWG as an xref to see how reference files are managed.

   ```
   XREF  →  Attach DWG
   ```

3. Open 1-12_Using_Layout_Tabs.dwg and review its layout tabs — plotting always happens from a layout with a page setup.

   ```
   OPEN → Layout tabs
   ```

4. Plot the active drawing to PDF at A3 size from the Plot dialog (printer: AutoCAD PDF, paper: ISO A3).

   ```
   PLOT → AutoCAD PDF → ISO A3
   ```

5. From Project Manager, choose Publish/Plot → Plot Project and select the sheets to output.

   ```
   Project Manager → Plot Project
   ```

6. Publish the project to a single multi-sheet PDF with Include Hyperlinks checked — cross-references become clickable links.

   ```
   AEPUBLISH → Multi-sheet · Hyperlinks
   ```

7. Open the PDF and click a parent's cross-reference to jump to its child; confirm the title block shows the plot date.

   ```
   Verify in PDF viewer
   ```


## Test it

The A3 PDF matches the layout exactly, and in the multi-sheet PDF clicking a cross-reference hyperlink jumps to the referenced component — the set is ready for standards-conformant submission.

---
*© 2026 Tertiary Infotech Academy Pte Ltd (UEN: 201200696W) · Technical Drawing with AutoCAD Electrical · Version v6.1*
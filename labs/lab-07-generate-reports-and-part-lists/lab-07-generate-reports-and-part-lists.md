# Lab 7 — Generate Reports and Part Lists

**Course:** Technical Drawing with AutoCAD Electrical (TGS-2023037466)  ·  **Topic 03:** Reviewing Technical Drawings for Strategic Relevance and Standard Compliance
**Maps to:** A6, K5 — extract BOM and wire lists, format them to house standards and place them on the drawing

## Goal

Run Bill of Material and Wire From/To reports across the project, tailor the fields, save a format file for repeat use, and insert the report as a table on the drawing — the part lists a checker reviews.

## What you'll build

A BOM table placed on the drawing plus a saved .SET format file and a CSV export of the report.

**Tools:** Reports · Bill of Material · Format files (.SET) · Tables · Attributes DWG

![Lab 7 workflow](workflow.png)

## Starter files (in this folder)

- `5-1_Working_with_Tables.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))
- `5-3_Using_Table_Links.dwg`  (source: [PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques](https://github.com/PacktPublishing/AutoCAD-2025-Best-Practices-Tips-and-Techniques))

## Step-by-step

1. Run the Reports tool on the Reports tab and choose Bill of Material, processing the whole project.

   ```
   AEAUDIT →  Reports → BOM
   ```

2. Adjust the report: include/exclude fields, reorder columns and rename field labels to your house standard.

   ```
   Change Report Fields
   ```

3. Save the settings as a format file so the same report can be re-run in one click next time.

   ```
   Save Format File (.SET)
   ```

4. Insert the report on the drawing as a table (Put on Drawing) using a table style.

   ```
   Put on Drawing · TABLESTYLE
   ```

5. Export the same report to a file for procurement (CSV/XLS).

   ```
   Save to File → CSV
   ```

6. Run a Wire From/To report and compare it against the wiring you created in Lab 4; open the supplied table drawings to see linked tables.

   ```
   Reports → Wire From/To
   ```


## Test it

The BOM table on the drawing matches the CSV export line for line, and re-running the report through your .SET format file reproduces the same layout — the part list is standard-compliant and repeatable.

---
*© 2026 Tertiary Infotech Academy Pte Ltd (UEN: 201200696W) · Technical Drawing with AutoCAD Electrical · Version v6.0*
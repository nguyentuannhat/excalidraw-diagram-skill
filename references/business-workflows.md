# Hand-drawn business workflows

Use this profile for business rules explained to product or operations stakeholders. Match the reading order, visual style, and level of detail of any approved reference supplied by the user.

1. Trace the decisions and outcomes in source material. Include fallback and manual review paths. Use terms familiar to the audience.
2. Place phases in columns from left to right with aligned headings and top rows. Use three columns when there are three natural phases. Read each column from top to bottom.
3. Use rounded blue rectangles for actions, pale amber diamonds for decisions, green outcomes for success, and red outcomes for exceptions. Use pale amber rectangles for short policy steps. Put longer rules in a lavender note beside or below the relevant step.
4. Place branch labels beside the arrow with a visible gap. Route exception lines inside the column. Use a named handoff when a connector would have to cross another column.
5. Use a 34–36 px title, 25–27 px phase headings, 17–20 px node text, and 15–16 px notes. Use white space between phases and leave room around accented letters.

Use the business workflow colors in [color-palette.md](color-palette.md). Use a white canvas, a 2 px stroke, roughness 1 for shapes and arrows, opacity 100, gently rounded connectors, and open arrowheads. Use Excalidraw fontFamily 1 for editable labels.

## Export two previews for comparison

Keep one editable `.excalidraw` scene with live text. Whenever delivering a preview, export both variants in the requested format. If both SVG and PNG are requested, export two of each.

| Variant | Filename | Typography |
|---|---|---|
| Default | `<name>-default.svg` or `<name>-default.png` | Preserve the editable scene's native Excalidraw fonts |
| Chalkboard | `<name>-chalkboard.svg` or `<name>-chalkboard.png` | Use the CSS font stack `"Chalkboard SE", "Comic Sans MS", Arial, sans-serif` |

Export the scene to SVG with the native renderer. Use that SVG as the base for both previews. For the Chalkboard copy, override the font family of diagram text in the SVG. Keep text anchors, positions, sizes, shapes, arrows, palette, and canvas bounds identical so the font is the variable being compared. If either font causes overflow, adjust the shared editable layout and export both again. Keep labels as editable text in the source scene.

For PNG, rasterize both SVG variants at the same scale. Use a device scale factor of 3 for slide-ready previews and wait for fonts to load before taking a screenshot. Run the Chalkboard export on a machine with Chalkboard SE installed. If the font is unavailable, report which fallback was used. SVG text can use a fallback font on another device.

Inspect both previews before delivery. Trace a success case, a fallback, and a manual review case. Check arrow endpoints, branch labels, diamond padding, and accented characters. Label both preview links so the user can choose.

# S3 Drawer Print Plan

Oct 22, 2026 · @Carlos

## What "3S" means

This plan builds one **S3 1F drawer with a Gridfinity grid roof**: S width, depth 3, one floor tall. In VAULT naming the letter is the width (S, M, L, XL) and the number is the depth in Gridfinity units, so S3 is 3 × 42 mm deep, the smallest drawer in the system. The manual's own exploded drawer diagram is exactly this S3 1F build.

- **Height:** I picked 1F because you didn't name one. 2F and 4F use the same parts list with the matching Box, Module and Facade swapped in (noted below).
- **Files:** the big parts come from the S Families folder. The small shared parts (key lock, springs, latch, runners, geared rails, caps, label, top handle) live in `01. DRAWERS/07. Universal` which is now in the project too, so every file in the table below is in VAULT.

## Parts to print

An S3 1F drawer is about 20 printed pieces from 16 files; the 5 large parts are in your VAULT folder and the rest come from `07. Universal`. Sizes are the measured STL bounding boxes as the files are oriented, so everything fits a 180 mm bed. Colours follow the manual's renders and are only cosmetic.

| # | Part | Qty | File | Folder | Size as oriented (mm) | Colour in renders |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | Module (the shell) | 1 | S3 Module 1F.stl | S Families/S3/Modules | 165 × 57 × 146 tall | Light grey |
| 2 | Box (the drawer tray) | 1 | S3 Box 1F.stl | S Families/S3/Boxes | 134 × 144 × 38 tall | Dark grey |
| 3 | Facade (front plate) | 1 | S1F (Turn On Supports).stl | S Families/Facades | 165 × 47 × 10 | Light grey |
| 4 | Grid Roof | 1 | S3 Grid Roof.stl | S Families/S3/Roofs | 124 × 124 × 146 tall | Light grey |
| 5 | Gridfinity Baseplate (optional, sits in the box) | 1 | S3 Baseplate.stl | S Families/S3/Gridfinity Baseplate | 126 × 134 × 4 | Orange or grey |
| 6 | Runner Guide | 2 | x3 Runner Guide.stl | Universal/Runners | small | Light grey |
| 7 | Runner Slide | 2 | x3 Runner Slide.stl | Universal/Runners | small | Dark grey |
| 8 | Runner Stopper | 2 | Runner Stopper.stl | Universal/Runners | tiny | Orange |
| 9 | S Geared Rail (optional, extra lock force) | 2 | S Rails.stl | Universal/Geared Rails | small | Orange |
| 10 | Springs | 1 pair | Springs.stl | Universal | small | Orange |
| 11 | Key Lock | 1 | Key (Turn On Supports).stl | Universal | small | Dark grey |
| 12 | Key Cap | 1 | Key Cap.stl | Universal | tiny | Light grey |
| 13 | Facade Cap | 1 | Facade Cap.stl | Universal | tiny | Light grey |
| 14 | Label | 1 | Label.stl | Universal | small | Light grey |
| 15 | Latch | 1 | Latch.stl | Universal | small | Orange |
| 16 | Top Handle (grid roof only) | 1 | Top Handle (Turn On Supports).stl | Universal | small | Dark grey |

**Other heights:** for 2F swap in S3 Module 2F (165 × 105 × 146), S3 Box 2F (86 tall) and S2F facade. For 4F use S3 Module 4f, S3 Box 4F and S4F facade; the 4F module is 201 mm along one side, so it needs a bed larger than 180 mm.

**Other roofs:** Table, Bowl and Under Table Mount roofs are in the same Roofs folder and skip the top handle. The manual says to put a 2F module directly under any roof when you add modifications.

**Optional extras:** 20 mm grid dividers (Universal/Grid Dividers), Gridfinity bins for the baseplate, and the depth-3 Manual Support (Universal/Manual Supports/x3) for steadier tall prints.

## Hardware to buy

One S3 1F drawer needs only six bolts, per the manual's drawer hardware page.

| Bolt | Qty | Used for |
| --- | --- | --- |
| M4 × 14 mm | 4 (6 for 2F or 4F) | Fixing the facade to the box |
| M6 × 50 mm | 2 | Top handle on the grid roof |

Flat-head bolts can usually be swapped for countersunk ones. No heat inserts, rods or bearings are needed for a plain drawer; those are for the mobile and backbone modifications.

## Printer, filament and settings

The manual says every part is tuned for standard slicer settings and basic PLA, so start there and change nothing until a test fit says otherwise.

- **Printer:** any printer with at least a 180 × 180 mm bed fits all S3 1F and 2F parts. The manual's slicer screenshots are Bambu Studio.
- **Filament:** basic PLA. The manual's main colour is Bambu PLA Basic Light Grey (10104). PETG or extra walls and infill make parts stronger. TPU is only for wheel tyres, not drawers.
- **Supports on:** every file named "(Turn On Supports)" needs them: the S1F facade, the key lock and the top handle.
- **Built-in supports:** the box has thin manual supports along its runner channels that you snap off after printing, so don't add slicer supports there.
- **Tall parts:** the module and the roofs print standing about 146 mm tall. Add the depth-3 Manual Support or a brim if your printer wobbles on tall prints.
- **Labels:** use the slicer's text tool to emboss your own text on the label before printing.

## Print order

Print the small lock parts first so you can test tolerances on your printer before committing to the big shell. Plates are grouped by colour to keep filament swaps down. Each plate is a ready-arranged .3mf in VAULT/01. DRAWERS/S3 1F Print Job on your Mac, laid out to fit a 180 mm bed.

1. **Fit-check plate:** S1F facade, key lock, key cap, facade cap and springs. Assemble the lock (steps 1 to 3 below) and check the key turns and springs back.
2. **Box plate:** S3 Box 1F on its own. Snap off its manual supports and check the runner channels are clean.
3. **Runner plate:** 2 runner slides, 2 runner guides, 2 runner stoppers, 2 S geared rails. Dry-fit the slides into the box.
4. **Module:** S3 Module 1F on its own, standing tall.
5. **Roof plate:** S3 Grid Roof, then the top handle (supports on).
6. **Finishing plate:** latch and label, then the optional S3 baseplate on its own plate (plate 7).

## Assembly

Steps 1 to 12 follow the 8-page Drawer Assembly guide; you need a mallet, a hex key and the 4 M4 bolts.

1. Push the key lock into the facade from the back, in the same orientation as the guide's picture.
2. Tap the key cap onto the key with a hammer or mallet.
3. Press both springs into the back of the facade, **flat side up**.
4. Snap the manual supports off the box's runner channels.
5. Optional: slide the top and bottom S geared rails into the box until they stop. Use them for extra locking force, or if you later put more than one box in a 2F or 4F module.
6. Slide the two runner slides into the box.
7. Turn the lock to its **open** position so the gears mesh, then bolt the facade to the box with 4 M4 × 14 mm bolts.
8. Slide the label into the facade and push the facade cap in.
9. Clip a runner guide onto each side of the box.
10. Slide the whole drawer into the S3 1F module.
11. Only once the box is fully inside, push the two runner stoppers into the module's side holes.
12. Flip the module over and press the latch into its slot underneath.
13. Bolt the top handle to the grid roof with 2 M6 × 50 mm bolts, fit the roof on top of the module, and drop the optional baseplate into the box. The guide doesn't illustrate this step; it comes from the manual's naming diagram.

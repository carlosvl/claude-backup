# Cyberpunk LED Helmet — 3D Print Plan

Oct 20, 2026 · @Carlos

## Overview

The helmet is a glossy black shell with bolt-on fins, a smoked visor, a red LED ring eye, lit jaw and cheek slots, and a fall of corrugated tubes off the back. Only the hard parts get printed; the tubes, visor and lights are bought.

No public STL of this exact design turned up, so pick one of three routes:

1. **Adapt an existing helmet (fastest).** The [Predator Spawn helmet](https://thangs.com/m/1240678) on Thangs is the closest base: it ships with dreadlock slots, a narrow eye cutout option for LEDs, pre-split parts and printed alignment pins. Kitbash the fins, ear clips and jaw onto it.
2. **Model it yourself (most faithful).** Sculpt over a standard head base in Blender or Fusion, using the two reference photos as front and side planes. Budget 15–30 hours of modeling.
3. **Hybrid.** Print a plain full-face sci-fi shell, then model only the add-ons (fins, side modules, jaw, eye bezel) as separate bolt-on parts. Good middle ground if you're new to modeling.

Everything below works for any route. It's sized for the Centauri Carbon 2: 256 × 256 × 256 mm bed, enclosed chamber, 350 °C nozzle.

## Print files (route 2, done)

The helmet is now modeled. The zip `cyberpunk_helmet_print_files.zip` from the chat has 17 STLs for a 62 cm head, already in print orientation. Every part is watertight and fits the 256 mm bed, and no two parts collide. A [3D viewer](https://claude.ai/artifact/AXCwgvYSqKYttvKfERdTTy) shows the assembly, with an exploded view and per-part sizes.

The model departs from the sections below in a few places:

- The shell is **4 pieces**: crown front, crown rear, lower front, lower back. They join with built-in lap flanges instead of pins and magnets.
- The wall is **2.4 mm**, printed with 5 walls, to keep weight down. Filament is about 1.1 kg for the helmet plus 0.3 kg for the visor buck.
- The tube sockets are **built into the crown rear**, so there is no separate manifold. There are 14 sockets sized for 17 mm OD loom.
- The fins and blades lock in with tabs and slots. The ear modules cover the side seams.
- The eye ring holder takes a **24-LED WS2812B ring, 66/52 mm**. 7 mm wire holes are already in the shell behind the pods and chin guard.
- The visor buck has a raised ridge that embosses the trim line, 8 mm outside the window.

Print `00_sizing_band.stl` first. To resize, run `python3 generate_helmet.py --head <cm>` (also `--tube`, `--ring-od`, `--wall`).

## Part breakdown

About 15 printed parts plus bought tubes, visor and LEDs.

| Part | Qty | Make it by | Notes |
| --- | --- | --- | --- |
| Dome (back of head) | 1 (split in 2–3) | Print | Carries the tube manifold and fin sockets |
| Faceplate frame | 1 (split in 2) | Print | Holds the visor; eye ring bezel sits on it |
| Jaw / chin guard | 1 | Print | Slotted grille for the red mouth LEDs |
| Front crown fins | 2 | Print | Tall swept blades; separate parts, socketed in |
| Side blades / antennas | 2–4 | Print | Thin and fragile; reinforce with rod |
| Ear modules + clips | 2 | Print | The boxy side units with buckle details |
| Cheek LED pods | 2 | Print | Hollow boxes with a diffuser window |
| Eye ring bezel | 1 | Print | Clear or white PETG to diffuse the ring |
| Rear tube manifold | 1 | Print | Sockets for the tubes |
| Side rod / pipe | 1 | Print or dowel | The cylinder on the left side |
| Visor | 1 | Buy + cut | Smoked PC or PETG sheet |
| Dreadlock tubes | 12–20 | Buy | Corrugated split loom |
| LEDs, battery, switch | — | Buy | See Visor and LED electronics |
| Emblem and warning decals | — | Vinyl | Use your own designs, not the seller's logo |

## Sizing and splitting

A full adult helmet runs roughly 260–300 mm deep and tall, so the shell won't fit the 256 mm bed in one piece. Plan on 4–6 shell pieces.

1. **Measure your head.** Circumference above the brow, ear-to-ear over the top, and brow-to-chin. Add 15–20 mm of clearance for padding.
2. **Scale the model.** Most helmet STLs are sized for about a 24.5" (62 cm) head. Scale uniformly to your circumference, never per-axis.
3. **Print a sizing ring first.** Slice a 10 mm band at the head opening, print it (about 1 hour) and try it on before committing to the full print.
4. **Split the shell.** Use the slicer's cut tool or Blender. A good split: dome front, dome back, faceplate left, faceplate right, jaw. Cut along existing panel lines so seams hide in the design.
5. **Add joinery.** Use dowel connectors or 5 × 5 mm printed pins at each seam, plus 2–3 pairs of 8 × 2 mm magnets where you want the faceplate removable.
6. **Keep fins separate.** Print them as their own parts with a square tab that slots into the dome. Flat on the bed they print stronger and cleaner than attached.

## Materials and slicer settings

Print the shell in black PETG; it's tougher than PLA and won't soften in a hot car. The enclosure also makes ASA an option if you want UV and heat resistance, with the filter running.

| Part group | Material | Layer | Walls | Infill | Supports | Orientation |
| --- | --- | --- | --- | --- | --- | --- |
| Shell pieces | PETG or ASA, black | 0.2 mm (adaptive on curves) | 3–4 | 10–15% gyroid | Tree, buildplate only where possible | Outer surface up, seam edge down |
| Fins and blades | PETG or PLA+ | 0.2 mm | 4–5 | 20% | Minimal | Flat on the bed |
| Jaw grille, pods | PETG, black | 0.16 mm | 3 | 15% | Tree | Slots vertical |
| Eye bezel, diffusers | Clear or white PETG | 0.2 mm | 2 | 100% or 0% | None | Flat |
| Pins, clips | PETG | 0.16 mm | 4 | 40% | None | Pin axis horizontal |

Use ElegooSlicer or Orca. Run speed near the 250 mm/s recommended figure rather than the 500 mm/s max for cleaner curved surfaces. If you have the CANVAS unit, print the red accent panels in red instead of painting them.

## Visor and LED electronics

The mirror-black face is a smoked visor behind the printed frame; the red glow is addressable LEDs behind diffusers, all on 5 V USB.

**Visor**

- Cut it from a smoked polycarbonate face-shield replacement or 0.75–1 mm smoked PETG sheet.
- For a compound curve, print a visor buck and heat-form the sheet over it with a heat gun or oven.
- Add one-way mirror window film on the outside for the reflective look; you see out, others don't see in.
- Seat it in a printed groove behind the faceplate frame and fix with screws or magnets so it can be replaced.

**Lights**

- Eye: a WS2812B ring (24–35 LEDs, about 70–85 mm across) behind the clear eye bezel.
- Jaw and cheeks: short WS2812B or plain red 5 V strip segments behind the grille slots.
- Controller: a small microcontroller (Seeed XIAO or Arduino Nano) for effects, or a USB LED controller for static red.
- Power: a slim USB power bank in a printed pocket at the back, plus an inline switch.
- Run wires along the inside of the shell in printed clips; leave the battery reachable without removing the visor.

## Dreadlock tubes and rear manifold

Don't print the tubes; corrugated split-loom wiring tubing gives the exact look, flexes, and costs a few dollars. Pro helmet makers do the same, modeling sockets sized for real tubing ([example](https://thangs.com/designer/Galactic%20Armory/3d-model/Marchion%20Ro%20Helmet%20-%203D%20Print%20Files-1058115)).

- Buy 1/2" (13 mm) black split loom; about 10 m covers 12–20 tubes at 50–90 cm each.
- Model a rear manifold: a curved plate with a staggered grid of sockets matched to the loom's outer diameter plus 0.3 mm.
- Glue the tubes in with E6000 or hot glue, or add a printed end cap with a set screw so they're replaceable.
- Vary lengths in a staggered fall, longest in the middle, like the reference.
- Cap the free ends with small printed plugs so they don't fray or snag.
- Bolt the manifold to the dome so tube weight pulls on the shell, not your head.

## Finishing

The gloss-black car-paint look comes from filling layer lines and clear-coating, not from the filament.

1. Glue seams with CA or PETG-safe epoxy; fill gaps with a 3D-printing filler or Bondo glazing putty.
2. Sand 120 → 220 → 400 grit.
3. Two or three coats of filler primer, sanding 400 between coats until the surface is glass-smooth.
4. Gloss black enamel, 2–3 light coats.
5. Mask and spray the red accents, or apply red vinyl stripes.
6. Gloss clear coat; wet-sand 1000–2000 and polish if you want it mirror-like.
7. Apply your own emblem and warning-style decals last, then a final clear mist to seal edges.
8. Paint the ear clips and buckle details satin black for contrast.

## Comfort and safety

This is a costume piece, not protective gear: don't wear it for biking, skating or anything with impact risk.

- Line the inside with 6–12 mm EVA or upholstery foam pads; adjust padding rather than reprinting for fit.
- Add vent slots in the jaw and under the fins, and consider a 30–40 mm 5 V fan to stop the visor fogging.
- Check your field of view on the sizing print; walking with limited peripheral vision needs a spotter in crowds.
- Keep the LED controller and battery off direct skin contact and away from foam, and don't leave it charging unattended inside the helmet.
- Weight adds up fast with tubes; aim under 1.5 kg and balance front fins against the rear tubes.

## Bill of materials and timeline

Expect roughly $90–150 in materials and 40–60 hours of printing on top of modeling and finishing. Costs are approximate.

| Item | Qty | Approx. cost (USD) |
| --- | --- | --- |
| Black PETG or ASA | 1.5–2 kg | 30–45 |
| Clear or white PETG | 100 g | 5 |
| Smoked PC face shield or PETG sheet | 1 | 10–20 |
| One-way mirror film | small roll | 8 |
| 1/2" black split loom | 10 m | 10–15 |
| WS2812B ring + strip, controller | 1 set | 15–25 |
| Slim USB power bank + switch | 1 | 10–20 |
| Magnets 8 × 2 mm | 20 | 6 |
| Filler primer, gloss black, clear coat | 1 can each | 25–35 |
| EVA foam padding | 1 sheet | 8 |

**Phase 1 — Model and fit (week 1)**

- [ ] Pick route: adapt, model, or hybrid
- [ ] Measure head and scale the model
- [ ] Print and test the sizing ring
- [ ] Split shell along panel lines and add pins and magnet pockets

**Phase 2 — Print (weeks 1–2)**

- [ ] Print shell pieces
- [ ] Print fins, blades, ear modules, pods and jaw
- [ ] Print eye bezel, diffusers and tube manifold
- [ ] Dry-fit everything before gluing

**Phase 3 — Assemble and finish (week 3)**

- [ ] Glue and fill seams
- [ ] Sand, prime, paint gloss black and red accents, clear coat
- [ ] Apply decals

**Phase 4 — Electronics, visor, tubes (week 3–4)**

- [ ] Form and fit the visor with mirror film
- [ ] Wire and test LEDs before closing up
- [ ] Install tubes in the manifold
- [ ] Add padding, vents and do a wear test

## Sources

- [Predator Spawn helmet (Thangs)](https://thangs.com/m/1240678)
- [Marchion Ro helmet, real-tubing sockets (Thangs)](https://thangs.com/designer/Galactic%20Armory/3d-model/Marchion%20Ro%20Helmet%20-%203D%20Print%20Files-1058115)
- [Elegoo Centauri Carbon 2 specs (Elegoo)](https://us.elegoo.com/collections/materials/products/centauri-carbon-2)
- [Centauri Carbon 2 recommended speed (Printer Hub)](https://printer-hub.ru/en/printers/elegoo-centauri-carbon-2)

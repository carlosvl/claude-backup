# Filament Guide for Bike and RC Car Parts

Oct 6, 2026 · @Carlos

## Quick picker

Three spools cover most bike and RC parts: PETG for rigid parts, TPU 95A for anything that flexes, and ASA for anything that lives in the sun. Pick by what the part has to survive.

| What the part has to do | Use | Why |
| --- | --- | --- |
| Bend, grip, or absorb hits (bumpers, plugs, protectors) | TPU 95A | Flexes and springs back instead of cracking |
| Stay rigid outdoors in sun and heat (mounts, brackets, guards) | ASA | Resists UV and holds shape in a hot car |
| Be a general rigid part, indoors or shaded (spacers, trays, clips) | PETG | Tough, cheap, and easy to print |
| Take high load, wear, or repeated impact (suspension arms, gears) | Nylon (PA) | Very tough and low friction |
| Be very stiff and light (chassis braces, servo and camera mounts) | PA-CF or PETG-CF | Carbon fiber adds stiffness and cuts flex |
| Be a test fit, jig, or shop organizer | PLA | Cheapest and most accurate, but softens in heat |

## The filaments

Each filament trades ease of printing against heat, impact, and weather resistance. Heat limits below are approximate, from general material knowledge, and vary by brand.

| Filament | Good at | Weak at | Heat limit (approx.) | Print difficulty |
| --- | --- | --- | --- | --- |
| PLA | Detail, accuracy, low cost | Heat, sun, impacts; brittle | 55–60 °C | Easy |
| PETG | Toughness, water and chemical resistance | Slightly flexible; strings; scratches easily | 75–80 °C | Easy |
| TPU 95A | Flex, grip, impact and abrasion | Not rigid; hard to get clean overhangs | About 80 °C | Moderate; prints slowly |
| ASA | UV, weather, heat, rigidity | Warps without an enclosure; fumes | 95–100 °C | Moderate |
| Nylon (PA) | Impact, wear, fatigue, low friction | Absorbs moisture; warps; flexes when thin | 100 °C and up | Hard |
| PA-CF / PETG-CF | Stiffness, low warp, matte finish | Less impact-tough than unfilled; abrasive | Higher than the base plastic | Moderate to hard |
| Polycarbonate (PC) | Heat and impact strength | Warps badly without a heated chamber | 110 °C and up | Hard |

Three points the table does not show:

- **Carbon fiber makes parts stiffer, not tougher.** A CF part resists bending but can crack on a hard hit where plain nylon would flex. It also needs a hardened steel nozzle, which the Centauri Carbon 2 has.
- **ABS is ASA without the UV resistance.** It costs a little less. Buy ASA unless the part stays indoors.
- **TPU hardness is a number.** 95A is firm like a skateboard wheel and prints reliably. 85A is softer and grippier but much harder to feed. Start with 95A.

## Bike parts

Print accessories, protection, and shop tools; do not print anything that carries your weight or stops the bike. ASA is the default for parts that stay on the bike outdoors.

| Part | Filament | Notes |
| --- | --- | --- |
| Bar-end plugs, grip collars | TPU 95A | Press fit; survives drops |
| Chainstay and frame protectors, cable rub guards | TPU 95A | Print thin and zip-tie or tape on |
| Light, computer, and GPS mounts | ASA or PA-CF | Add a TPU shim between mount and bar to stop slipping and rattle |
| Bottle cage | ASA or nylon | Nylon flexes without cracking; PETG works but fatigues sooner |
| Fender extensions and mud flaps | ASA (rigid), TPU (flap) | TPU flap will not snap if it hits the tire |
| Cable guides, clips, non-structural spacers | PETG or ASA | PETG is fine out of direct sun |
| Pump, tool, tube, and CO2 holders | PETG or ASA | Use TPU straps instead of rigid clips where you can |
| Brake pad spacers, bleed blocks | PETG | Cheap to reprint to exact size |
| Bearing drifts, chain keepers, work-stand helpers | PLA or PETG | Shop tools see little heat; PLA is fine |

**Do not print:** stems, handlebars, seatpost or saddle clamps, brake levers or brake mounts, axle and dropout parts, crank or pedal parts, helmet parts, or child-seat parts. Printed parts are weakest between layers and can snap without warning.

Two habits make bike parts last:

- Orient the part so the load runs along the layers, not across them. A clamp printed lying flat is far stronger than one printed standing up.
- Keep PLA and PETG away from disc brake calipers and rotors, which get hot enough to soften them.

## RC car parts

Use TPU for anything that takes the crash, nylon for anything that carries the load, and keep PLA for stands and scale details. Expect printed load parts to break sooner than molded ones; the advantage is a cheap reprint.

| Part | Filament | Notes |
| --- | --- | --- |
| Bumpers, skid edges, body savers | TPU 95A | Thick walls with 15–25% gyroid infill cushion best |
| Body posts and wing mounts | TPU 95A or nylon | TPU bends in a rollover instead of shearing |
| Shock boots, receiver box seals, wire grommets | TPU 95A | Thin walls; print slowly |
| Battery straps | TPU 95A | Tray itself in PETG or ASA |
| Crawler tires and tire inserts | TPU 85A–95A | Softer grips better but is harder to print |
| Suspension arms, hub carriers, steering knuckles, shock towers | Nylon (PA) | PETG is a cheap first try; plain nylon for bashers |
| Chassis plates, braces, servo mounts | PA-CF or PETG-CF | Stiffness matters more than impact here |
| Gears and diff covers | Nylon (PA) | Fine for low power; printed spur gears wear faster than molded |
| Motor mounts and parts next to the motor or ESC | PA-CF or PC | Motors run hot enough to soften PETG; metal is better |
| Beadlock rings, wheels for crawlers | PETG or nylon | Low speed only |
| Body shells, roof racks, light buckets, scale details | PETG or ASA | ASA if the car sits in the sun |
| Car stands, setup gauges, parts trays | PLA | No heat or impact to worry about |

Basher or racer changes the nylon choice. A basher that lands jumps wants plain nylon, which flexes and recovers. A racer or crawler that needs precise geometry wants PA-CF, which holds its shape but cracks on a hard enough hit.

## Printing and handling on the Centauri Carbon 2

The printer's 350 °C hardened nozzle and 110 °C bed reach every filament here; the limits are moisture, warping, and how TPU is fed. Temperatures below are typical ranges and approximate, so the spool label wins when they differ.

| Filament | Nozzle (°C) | Bed (°C) | Door and lid | Dry first? |
| --- | --- | --- | --- | --- |
| PLA | 200–220 | 55–65 | Open, to avoid heat clogs | Rarely needed |
| PETG | 230–250 | 70–85 | Either | If it strings or pops |
| TPU 95A | 220–240 | 40–60 | Open | Always |
| ASA | 240–260 | 90–110 | Closed | Helpful |
| Nylon and PA-CF | 260–300 | 80–100 | Closed | Always, and print from a dry box |
| PC | 270–310 | 100–110 | Closed | Always |

- **TPU needs an adapter on the Combo.** Elegoo says TPU requires its Flexible Filament Printing Adapter, with the multicolor unit bypassed. A [Notebookcheck review](https://www.notebookcheck.net/Elegoo-Centauri-Carbon-2-3D-printer-review-Lot-of-features-for-not-a-lot-of-money.1239803.0.html) printed TPU cleanly without it, but needed profile tuning. Print TPU slowly, around 20–40 mm/s.
- **Preheat for ASA.** The same review had ASA lifting off the plate until the bed was preheated at 110 °C for 10 minutes. Keep the door shut and avoid large flat parts at first.
- **There is no built-in dryer.** The multicolor unit does not dry filament, so wet TPU or nylon will string, bubble, and print weak. A separate dryer fixes this.
- **PC is for small parts only.** With no chamber heater, large polycarbonate parts will warp.
- **Ventilate for ASA and nylon.** Both give off fumes. The printer has a filter, but run it in a garage or a room you can air out.
- **Stock profiles are tuned for PLA and PETG.** Expect to adjust settings for TPU and ASA. A temperature tower and a flow test on each new spool save failed prints.

## What to buy first

Start with PETG and TPU, add ASA once PETG prints cleanly, and leave nylon until you have a dryer.

1. **PETG, 1 kg in black or grey.** Your default for rigid parts and the easiest way to learn the printer.
2. **TPU 95A, 1 kg.** Bumpers, protectors, plugs, straps, and liners.
3. **ASA, 1 kg.** Outdoor bike mounts and anything left in a hot car.
4. **A filament dryer.** Needed for TPU and nylon; it also rescues old PETG.
5. **PLA, one cheap spool.** Test fits, jigs, and shop tools, so you do not waste the good filament on prototypes.
6. **Nylon or PA-CF, later.** Buy it when a PETG suspension arm or mount breaks and you know which part needs it.

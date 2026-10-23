---
name: "persist-howto-as-md"
description: "Use when giving hardware setup, wiring, calibration, product configuration or other lasting how-to steps: save them as a markdown file in the project and link it."
---

# Persist how-to answers as markdown

(Imported from Cursor: global rule `persist-howto-as-md.mdc` + skill `persist-howto-as-md`.)

## When this applies

Use whenever the user asks for (or you produce) lasting procedural guidance, including:

- Hardware setup / calibration (pots, voltage/current limits, DIP switches)
- Wiring or assembly step-by-step instructions
- Product datasheet procedures turned into actionable checklists
- "How do I set X on this module?" style questions
- Part verification that ends with keep/buy instructions worth saving

## Required behavior

1. **Always create or update an `.md` file** in the relevant project folder (prefer existing docs trees like `docs/`, `hardware/`, `README` siblings). Do not leave the full procedure only in chat.
2. **Name it clearly** after the device or task (e.g. `CYWHRVZSF-BUCK-SETUP.md`, `WIRING-FOO.md`).
3. **Link it** from the nearest parent doc (README, MOBILE-POWER, etc.) when one exists.
4. **Answer in chat briefly** and point to the file path; put the durable detail in the markdown.
5. If a good file already exists, **update it** instead of duplicating.

## File content

Include: prerequisites, what is / isn't adjustable, numbered steps, target values, a do/don't table, and a short checklist. Match the project's existing doc tone.
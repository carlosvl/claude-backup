# Claude account backup

Work and setup from Carlos's old Claude account, saved on 2026-10-23 before
moving to a new account. Project work for NCYD and Raspberry-PAB lives in those
repos' `claude/` folders; this repo holds everything else.

## What's here

| Folder | Contents |
|--------|----------|
| [memory/](memory/memory-export.md) | Everything Claude remembered, ready to paste into the new account |
| [3d-printing/](3d-printing/) | S3 Drawer Print Plan, Cyberpunk LED Helmet print plan and 3D viewer, Filament Guide for bike and RC parts |
| [travel/](travel/savannah-trip-plan.md) | Savannah Trip Plan |
| [skills/](skills/) | The `persist-howto-as-md` skill, plus upload-ready ZIPs of all three custom skills |
| [account/](account/connectors.md) | Connectors, Mac setup, skills and scheduled tasks to recreate |

Elsewhere:

- **carlosvl/NCYD** `claude/`: General Mills and Nerds partnership decks, the
  NCYD home page design, the Stripe subscriptions and duplicate-matching docs,
  the MTB Devo overview, NCYD notes.
- **carlosvl/Raspberry-PAB** `claude/`: the two MCA skills and the Weekly CI
  health check scheduled task.

## Migration checklist

**Before closing the old account**

- [ ] Export your data: Settings → Privacy → Export data. The emailed link expires after 24 hours.
- [ ] Download `cyberpunk_helmet_print_files.zip` (17 STLs plus `generate_helmet.py`) from the helmet chat. It was a chat file, not an artifact, so it isn't backed up here.
- [ ] Export the two partnership decks as PowerPoint or PDF, and the NCYD home page as an image or PDF.
- [ ] Export the Stripe subscriptions doc and the MTB Devo overview as PDF. Their charts and diagrams didn't come through in markdown.
- [ ] Copy anything from claude.ai Projects (instructions and knowledge files) you want to keep. Those weren't reachable from here.
- [ ] Push the MCA what-if code from the Mac (see Raspberry-PAB `claude/README.md`).

**In the new account**

- [ ] Sign the Claude desktop app on the Mac into the new account, and re-add your connected folders.
- [ ] Reconnect connectors, including GitHub ([account/connectors.md](account/connectors.md)).
- [ ] Upload the three skill ZIPs from `skills/zips/`.
- [ ] Paste [memory/memory-export.md](memory/memory-export.md) and ask Claude to remember it.
- [ ] Recreate the Weekly CI health check scheduled task.
- [ ] Rebuild any decks or docs you still need from the saved files.

**After everything works**

- [ ] Cancel the old plan if it's paid, then delete the old account.

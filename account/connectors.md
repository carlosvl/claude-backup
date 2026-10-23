# Connectors and setup to recreate

What was connected in the old Claude account on 2026-10-23. None of these carry
over; connect each again in the new account (Settings → Connectors) and sign in.

## Connectors

| Connector | Used for |
|-----------|----------|
| Gmail | Reading and drafting email |
| Google Calendar | Schedule and events |
| Google Drive | Files |
| Google Docs | Editing Google Docs |
| Google Sheets | Editing Google Sheets |
| Google Slides | Editing Google Slides |
| Stripe | NCYD payments and subscriptions |
| Resy | Restaurant reservations |
| GitHub | Access to carlosvl repos (needed for the CI scheduled task and to read these backups) |

## On the Mac (desktop app)

These are set up on the Mac itself, so they should still be there after you sign
the Claude desktop app into the new account. Check each one works:

- Local tools: raspberry-ssh (the Pi), react-mcp, salesforce-dx, vagrant-mcp.
- Claude in Chrome extension: sign it into the new account.
- Connected folders: add them again from the "+" menu in the desktop app.

## Custom skills

Ready-to-upload ZIPs are in [`skills/zips/`](../skills/zips/). In the new account
go to Customize → Skills, click **+**, choose **Create skill**, then **Upload a
skill**, and upload each ZIP.

| Skill | ZIP | Source |
|-------|-----|--------|
| `persist-howto-as-md` | `skills/zips/persist-howto-as-md.zip` | this repo, `skills/persist-howto-as-md/` |
| `mca-state-qualifiers` | `skills/zips/mca-state-qualifiers.zip` | carlosvl/Raspberry-PAB, `claude/skills/mca-state-qualifiers/` |
| `mca-state-whatif` | `skills/zips/mca-state-whatif.zip` | carlosvl/Raspberry-PAB, `claude/skills/mca-state-whatif/` |

## Scheduled tasks

| Task | Saved in |
|------|----------|
| Weekly CI health check (Mondays 8:59 AM Central) | carlosvl/Raspberry-PAB, `claude/scheduled-tasks/weekly-ci-health-check.md` |

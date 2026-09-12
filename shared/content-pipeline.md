# Content pipeline — Dropbox → Pinterest

## Roles
- **TK:** create assets and copy in Dropbox; mark ready via a handoff
- **Grok:** pick up ready packs, schedule/publish to Pinterest Business
- **James:** brand/voice decisions and final approval when needed

## Dropbox convention (proposed)
Put ready packs under something like:

`/RJDS/Content/Pinterest/ready/YYYY-MM-DD-<slug>/`

Each pack should include:
- image(s) or video to pin
- `pin.md` with title, description, destination URL, board name, optional hashtags
- optional `schedule.md` with preferred publish time (BST)

## Handoff
When a pack is ready, TK (or James) drops a file in `handoffs/`:

`YYYY-MM-DD-pinterest-<slug>.md`

Using the handoff template: From TK → To Grok, Done when = pin live (or scheduled) + link logged.

## Status
- Grok logs Pinterest work in `grok/status.md`
- TK logs creation work in `tk/status.md`

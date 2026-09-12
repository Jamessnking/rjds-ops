# Handoff: B-Roll Packs → Dropbox (licensed / AI — not Pinterest scrape)

**From:** TK / Grok (updated)  
**To:** Izzy  
**Date:** 2026-09-12  
**Priority:** Medium — batch background job  
**Status:** In progress (Pinterest scrape path closed)

---

## Decision

Do **not** scrape Pinterest (or similar) for images/video to republish. ToS + copyright risk — closed with James.

Use instead:
1. **AI generation** (Pyxa) for consistent avatars / reference faces and generated B-roll where appropriate
2. **Licensed stock** only (Pexels, Pixabay, or other clear-licence sources) when real footage is needed

---

## Objective

Build B-roll packs for social from the cinematic prompts doc, stored in Dropbox for Reels / Pinterest-adjacent content — without scraping Pinterest.

---

## Source File

- **Google Drive file:** broll_ai_video_prompts.md
- **File ID:** 1s1sb0mh4Dqw4MEc9zoSUYPE8Jcgk6vAXjAyBD540CI0
- **View link:** https://docs.google.com/document/d/1s1sb0mh4Dqw4MEc9zoSUYPE8Jcgk6vAXjAyBD540CI0/edit
- Drive MCP may be broken — use browser or export if needed

---

## Current path (Izzy)

- [x] Topics queue built from the Drive prompts doc
- [ ] Pyxa consistent-avatar / reference-face generation → Dropbox **B-Roll-Master** (or agreed folder under Side Hustle Brain)
- [ ] Per-topic B-roll packs as AI or licensed stock
- [ ] Log progress; pause if rate-limited

---

## Done when

- Topics have usable B-roll assets in Dropbox under the agreed structure
- No Pinterest-scraped media in the packs
- Handoff marked complete + note in Izzy/TK status

---

## Closed approach (do not reopen without James)

- ~~Search Pinterest and download images for republication~~

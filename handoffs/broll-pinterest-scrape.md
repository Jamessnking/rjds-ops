# Handoff: B-Roll Pinterest Scrape → Dropbox

**From:** TK  
**To:** Grok  
**Date:** 2026-09-12  
**Priority:** Medium — batch background job

---

## Objective

James has a Google Drive doc with 1,000 cinematic B-roll prompts (100 topics x 10 camera variants each). For each topic, search Pinterest for images that visually match the description and save them to Dropbox. These will be used as B-roll snippets in social content.

---

## Source File

- **Google Drive file:** broll_ai_video_prompts.md
- **File ID:** 1s1sb0mh4Dqw4MEc9zoSUYPE8Jcgk6vAXjAyBD540CI0
- **View link:** https://docs.google.com/document/d/1s1sb0mh4Dqw4MEc9zoSUYPE8Jcgk6vAXjAyBD540CI0/edit

---

## Structure of the File

- 100 topics (e.g. "Weather changes", "Seasons changing", "City at night")
- Each topic has 10 prompts with shot type + lighting + mood + subject description
- For Pinterest searching, use the **topic name** as the primary search query — no need to search all 10 variants separately

---

## Your Task (Per Topic)

1. Take the topic name as the Pinterest search query (e.g. "rain city street cinematic", "autumn leaves falling drone shot")
2. Search Pinterest for 5-10 high-quality images matching that visual vibe
3. Download the images
4. Save to Dropbox under: Side Hustle Brain/B-Roll/{topic_name}/
5. Move to the next topic

---

## Notes

- Prioritise cinematic, clean, high-res images
- Skip low quality / watermarked images where possible
- Work through topics in order (1 to 100)
- If Pinterest blocks or rate-limits, pause and log how far you got in grok/status.md
- Update grok/status.md with progress as you go

---

## Status

- [ ] In progress  
- [ ] Complete

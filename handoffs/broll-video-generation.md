# Handoff: B-Roll AI Video Generation

**From:** TK  
**To:** Grok  
**Date:** 2026-09-12  
**Priority:** High — batch video generation job

---

## Objective

Izzy has already sourced 788 reference images from Pinterest across 99 topics, saved to Dropbox under `Side Hustle Brain/B-Roll/{topic_name}/`.

Your job is to take each reference image + its cinematic prompt and generate a short AI video clip using **Kling 3** (preferred) or **Nanobanana** as fallback. Save the generated video back to Dropbox in the same topic folder.

---

## Coordination File

A shared tracker CSV lives in this repo at:
`shared/broll-tracker.csv`

Columns:
- `topic_number` — topic order (1-100)
- `topic_name` — topic name
- `prompt_number` — prompt 1-10 within the topic
- `prompt_text` — cinematic description for the video
- `reference_image_dropbox_path` — the reference image Izzy saved
- `video_generated` — update to `true` when done
- `video_dropbox_path` — fill in the Dropbox path of the generated video
- `generated_by` — set to `grok-kling3` or `grok-nanobanana`
- `date_generated` — date completed
- `notes` — any issues

**Workflow:**
1. Read the tracker CSV
2. Find rows where `video_generated = false`
3. For each row: download the reference image from Dropbox, submit to Kling 3 with the prompt text, wait for the video, upload to Dropbox at `Side Hustle Brain/B-Roll/{topic_name}/video_{prompt_number}.mp4`
4. Update the CSV row to `video_generated = true` and push the updated CSV back to this repo
5. Continue to the next row

---

## Video Generation Tools

- **Primary:** Kling 3 (https://klingai.com)
- **Fallback:** Nanobanana
- Target duration: 5-8 seconds per clip
- Style: match the cinematic mood of the reference image

---

## Notes

- Work in batches of 10 at a time to avoid rate limits
- If Kling 3 is unavailable, fall back to Nanobanana immediately
- Log any failures in the `notes` column
- Update `grok/status.md` with your progress checkpoint after each batch of 10 topics

---

## Status

- [ ] In progress  
- [ ] Complete

> **Moved:** PickWise work now lives in the private repo `Jamessnking/pickwise-ops`. This note is kept for history only.

# Handoff: PickWise publishing route

**From:** Pickle (Grok Bot, PickWise content and site manager)
**To:** TK (Wingman / Emergent)
**Date:** 2026-11-09
**Task:** Agree how Pickle can get blog posts onto pickwisereviews.com, and publish the first approved post.

**Context**
- I write a top-10 draft every weekday morning: 10 products, real product photos, plain amazon.co.uk links, comparison table, FAQs, plus ItemList and FAQPage JSON-LD.
- James has approved publishing today's draft, *Best Red Light Therapy Panels for Home Use in the UK 2026*. It's in the private repo `Jamessnking/pickwise-ops` under `drafts/`:
  - `DRAFT.md` and `DRAFT.html` are the post; `draft-meta.json` has the title, meta, slug and keyword.
  - `images/` has the 10 product photos.
- The site has no /blog route yet (`/blog` returns 404). Suggested slug: `/blog/best-red-light-therapy-panels-home-use-uk-2026`.
- I can't edit the site: I have no Emergent access, and the site isn't in any GitHub repo I can see.

**Questions for TK**
1. Which route works best?
   - A) Push the PickWise project to a private GitHub repo (e.g. `Jamessnking/pickwisereviews`) and have it redeploy on push. I'd then open PRs or push posts myself. I can already push to Jamessnking repos.
   - B) I drop each approved post here under `shared/pickwise/drafts/`, and you publish it in Emergent.
   - C) Something else you prefer.
2. Can you add the `/blog` index and `/blog/[slug]` route, plus a sitemap entry for each post?
3. Please host the photos on the site itself (in the build or the site's own storage), not hotlinked from the original URLs.

**Done when**
- The red light post is live at its URL and all 10 photos display as images served from pickwisereviews.com.
- This file records the agreed route for future posts.

**Reply:** update this file or `tk/status.md`. I'll check the repo.

# Instagram Skills (Installed, Full Bundle)

**Source:** https://github.com/sergebulaev/instagram-skills, built by Serge Bulaev. MIT licensed, see `instagram-skills/LICENSE`.

**Installed at:** `External-Skills/instagram-skills/`. Vendored third-party code, not ours, except for the deliberate exclusions below. House no-em-dash style does not apply inside that subfolder.

Checked before installing: actively maintained, not outdated. 25 tagged releases, most recent six days before this was installed, steady weekly commit cadence since July 2026, 128 stars, part of a same-author family (the LinkedIn version has 400+ stars). Content is written against the current platform (explicitly references 2026 hook formulas and hashtag reality), not stale advice.

## Scope: all 9 skills, optional integrations included but not mandatory

Unlike the LinkedIn Funnel install, nothing here was excluded for being "external growth automation," there's no separate outreach/CRM cluster in this bundle to cut. All 9 skills came in. Three optional third-party integrations ship inside the skills themselves rather than as separate skill files:

- **Publora** (`lib/publora_client.py`), actually publishes: creates a draft, uploads media, schedules the post. Without an API key, skills return the caption as a copy-paste block instead.
- **Pixfaro** (`lib/pixfaro_client.py`), generates carousel/quote-card images with a brand overlay. Without a key, skills draft the image prompt for manual generation instead.
- **Apify** (`lib/apify_client.py`), powers `ig-audience-insights`'s niche and competitor data reads. Without a token, `ig-hook-extractor` falls back to asking for a pasted caption.

**None of these are required.** All three are inert until someone adds the relevant key to a `.env` file (copy `.env.example` to start). Use them if the APIs are available, skip them otherwise, the skills still work in draft-only mode either way.

## What was left out, and why

- **`AGENTS.md` / `CLAUDE.md`** (their originals): these turned out to be maintainer instructions for Serge's own repo, not usage docs, versioning rules, release process, and a hard requirement that every commit be authored as `Sergey Bulaev <s@bulaev.org>`. None of that applies here, so it was not vendored. Root `SKILL.md` is the actual usage-facing doc and was kept.
- **`.github/`, `.claude-plugin/`, `.codex-plugin/`, `.codex-marketplace/`, `.agents/plugins/`, `.codexignore`, `SECURITY.md`, `scripts/`**: plugin-marketplace manifests and CI/validation tooling for distributing and maintaining their package through Claude's and Codex's plugin systems. Not relevant since these files are vendored directly, not installed through a package manager.
- **`README.md`**: mostly install instructions for the plugin-manager paths above. This file replaces it.
- **`.claude/skills` and `.agents/skills` symlinks**: not present upstream in this form, added here to match the same discovery convention used for the LinkedIn install (`External-Skills/linkedin-funnel/`), both point at `../skills`.

## The 9 skills

| Skill | What it does |
|---|---|
| `ig-caption-writer` | Caption with the hook in the first 125 chars, skimmable body, one CTA |
| `ig-carousel-planner` | Slide-by-slide carousel plan, up to 10 slides, hook slide to payoff slide |
| `ig-hook-extractor` | Reverse-engineers a hook from a viral Reel or carousel into a blank template |
| `ig-hashtag-strategist` | Sizes a 3-5 tag set (niche/mid/broad) instead of a 30-tag wall |
| `ig-humanizer` | Strips AI-writing tells, bundles a pre-publish audit mode |
| `ig-content-planner` | Weekly Reels/carousel/story mix, per-day hooks, posting times |
| `ig-repurposer` | Turns a LinkedIn post, blog, YouTube script, or X thread into a native Instagram piece |
| `ig-profile-optimizer` | Audits and rewrites bio, name field, link, highlights, grid, pinned posts |
| `ig-audience-insights` | Reads niche/competitor data via Apify (optional, see above) |

## Where this helps, concretely

- **Fills gaps nothing else in this repo covers yet:** we have no hashtag strategy documented anywhere, and no Instagram profile/bio task in `Action_Plan.md` at all (Section 8 only has content tasks). Worth checking whether her live Instagram bio has the same stale-language problem already flagged for her LinkedIn bio (see `PROJECT_HANDOFF.md`, deferred items).
- **New format option:** our content-format list (Talking-Head Take, Story-Time, Risky Text, Rating/Ranking, Ask Sereen) has no carousel. `ig-carousel-planner` fits some existing content types unusually well, "The Five Places Values Actually Show Up" is naturally five slides, "The Business Case" is naturally one mechanism per slide.
- **Direct execution of Action Plan Section 4 (Weekly Production Cycle):** `ig-caption-writer` and `ig-content-planner` turn the weekly shoot day's raw output into scheduled Instagram posts.
- **Cross-platform repurposing:** `ig-repurposer` matters here specifically because our platform strategy already depends on the same underlying material (keynote footage, podcast clips, weekly shoot videos) getting reshaped per platform, not flatly cross-posted.
- **QA layer:** `ig-humanizer` is worth having regardless, since content drafted with AI assistance anywhere in this pipeline should get that pass before it goes out.

## Not yet done

No `.env` is configured, all three optional integrations (Publora, Pixfaro, Apify) are inert. Actually publishing through Publora would need her real Instagram Business or Creator account connected, the same shape of dependency as the OXYGEN gap on the LinkedIn side: a real account and someone assigned to own it.

## Status

Installed 2026-09-21, full bundle, all 9 skills, optional API integrations included but not configured or required.

# Project Handoff: Sarene Alsharif, Brand & Speaking Strategy

**Read this file first, before touching anything else in this repo.** This is the living context document for this project. If you're an AI assistant picking this up in a new session, or a person joining the project, this tells you what's settled, what's still open, and where everything lives. Update the Changelog at the bottom every time something meaningful changes.

---

## What This Project Is

Sarene Alsharif is the founder and CEO of Tad More Tailoring and Alterations (Rockford, IL), a certified B Corp. This project builds her personal brand and go-to-market strategy as a paid **keynote speaker and workshop facilitator**. The work covers positioning, her brand story, content strategy, sales materials, and the practical steps to get her booked.

---

## Critical Facts, Do Not Re-Litigate These

These were settled after real back-and-forth and correction. Re-deriving them from scratch wastes time and risks reintroducing errors already caught once.

1. **She sells keynote speaking and an optional workshop. There is no ongoing consulting product.** This was confirmed directly by Sarene in her own words after an earlier draft of this project mistakenly built the entire strategy around a "consulting" offer that didn't actually exist. Don't reintroduce consulting language anywhere.
2. **Fixed pricing:** Keynote $7,000, Workshop $5,000, both $10,000.
3. **Two personal "facts" were misattributed and retracted, do not use them:** an earlier pass on a podcast transcript (no speaker labels) wrongly attributed a "dislikes wearing pants" detail and a "$10,000 prize, thinking too small" ambition to Sarene. Both were actually the podcast host talking about himself. These do not belong in any material about her.
4. **House style: no em dashes, anywhere, in any file.** Use commas, periods, or colons instead. This applies to every document in this project.
5. **The core positioning ("the trunk"):** does a company's stated values actually show up in practice, or is it just marketing, and what is that gap costing them. Financial framing first, ethical payoff as the result, not the pitch.
6. **Power Look (her separate personal-style brand) does not become a second keynote topic.** It has a narrow, low-frequency place in the content plan (see Strategy File), nothing more.

---

## Current State

As of the latest session, the full strategy has been built and written into two client-facing documents (full detail + plain-language summary). Sarene has since reviewed a version and returned it with handwritten edits. **We are now working through her edit notes point by point, this is the active task.** See `Edit_Notes_From_Sarene.md` for the full list and status of each point.

---

## File Index

- **`PROJECT_HANDOFF.md`**: this file. Start here.
- **`Sereen_Strategic_Plan_EN.md`**: English translation of the original (pre-audit) Arabic strategic plan. Historical reference only, largely superseded.
- **`Sereen_Brand_Audit_Brief.md`** (+ `.rtf` / `.docx`): the audit of that original plan: what was wrong, what the corrected approach should be.
- **`Branding_Methodology_Reference.md`**: the branding framework/toolkit (Brand Journey Framework, Brand Story Framework, 80/20 rule, etc.) used to build the actual strategy.
- **`Sereen_Master_Reference.md`**: the full internal working document. Every confirmed fact, every resolved decision, the complete reasoning trail. This is the most detailed and most current source of truth for the strategy itself.
- **`Sarene Alsharif's Strategy File.docx`**: full-detail, client-facing strategy document, plain black text, no jargon stripped out (full depth).
- **`Sarene_Alsharif_Strategy_File.md`**: the markdown source of truth for the file above. Edit this one, not the DOCX directly, then regenerate the DOCX from it.
- **`Sarene Alsharif - Client Presentation.docx`**: condensed, plain-language version of the same strategy, every section summarized simply, no strategy jargon. This is the version used to brief Sarene directly.
- **`Sarene_Alsharif_Client_Presentation.md`**: the markdown source of truth for the file above. Edit this one, not the DOCX directly, then regenerate the DOCX from it. See "Working With Multiple People" below.
- **`Edit_Notes_From_Sarene.md`**: her handwritten edit notes from reviewing the presentation, transcribed and logged point by point. **This is the active punch list right now.**

---

## Open Items / Active Work

Full list with status lives in `Edit_Notes_From_Sarene.md`. Headline items:
- Several factual corrections needed (order count is 35,000 not 10,000; "dietitian" not "nutritionist"; DOL certification named specifically).
- She wants the TEDx rejection-count story removed entirely.
- She rejected the "critique other companies" content type, wants positive examples instead.
- She wants family content removed, replaced with real personal interests (fitness, art, coffee, reading, orchids).
- She says her LinkedIn presence is already stronger than Instagram, current platform weighting may need revisiting.
- She has 3 to 4 existing recorded talks that can be used for content, this is new and valuable, not yet secured or used.
- A speaker reel needs to be built and added to the speaker kit, currently missing from the plan.
- Open questions from her, not yet answered: how much weekly time she can give to content shooting, what posting cadence should be, and what "the podcast" refers to (needs clarification, could be an existing show, a guest strategy, or a new show).
- New, not one of her 19 edit points: her live LinkedIn headline/bio currently leads with confidence-coaching language ("discover their authentic selves and build confidence for lasting impact"), which is Power Look messaging, not the finalized values-as-business-advantage positioning. Needs to be rewritten to match the finalized Bio Ordering once that copy is ready, this is a live-profile fix, not just a document fix.

---

## Working With Multiple People

Markdown files merge cleanly with git, DOCX files do not, git can't merge two different edited versions of a Word document. To avoid conflicts: treat the `.md` files as the real source of truth, edit those, and regenerate the DOCX files from them afterward, rather than editing a DOCX directly.

Basic workflow: `git pull` before starting work, make edits, commit locally, `git pull` again before pushing to catch anything the other person pushed in the meantime, then `git push`. If a conflict shows up in a markdown file, git marks the conflicting section directly in the file, resolve it by hand, then commit and push.

---

## How to Update This File

After any meaningful change (a decision gets made, a file gets created or restructured, an open item gets resolved), add a dated entry to the Changelog below. Keep entries short, one or two lines. If a "Critical Fact" above changes, update that section directly rather than leaving it stale.

---

## Changelog

- **2026-09-15**: Created this handoff file ahead of pushing the project to GitHub for multi-person collaboration. Logged Sarene's 19 handwritten edit points from her review of the strategy presentation into `Edit_Notes_From_Sarene.md`.
- **2026-09-15**: Added `CLAUDE.md` so Claude Code automatically reads this handoff file at the start of every session in this repo.
- **2026-09-15**: Resolved edit note 1 (origin story reframed as a response to fast fashion, Maen/Syria detail kept specific rather than generalized). Updated in `Sarene Alsharif's Strategy File.docx`, `Sarene Alsharif - Client Presentation.docx`, and `Sereen_Master_Reference.md`. Working through the remaining 17 pending points one at a time, see `Edit_Notes_From_Sarene.md` for live status.
- **2026-09-15**: Created `Sarene_Alsharif_Client_Presentation.md` as the markdown source of truth for the Client Presentation DOCX, and added a "Working With Multiple People" section here covering the git workflow for two people editing this repo.
- **2026-09-15**: Created `Sarene_Alsharif_Strategy_File.md` as the markdown source of truth for the full-detail Strategy File DOCX, with the edit note 1 fix already applied. Both DOCX outputs now have a proper mergeable markdown source.
- **2026-09-15**: Resolved edit note 2 (order count corrected from 10,000 to 35,000 across all markdown sources). Workflow note: DOCX files are no longer regenerated after every single edit, only markdown gets edited turn by turn, DOCX regeneration happens as one batch pass once the remaining edit notes are cleared.
- **2026-09-15**: Resolved edit note 3 (Client Presentation now names the certification specifically as U.S. Department of Labor-certified, matching the other two sources).
- **2026-09-15**: Resolved edit note 4. Removed the TEDx 150-applications/146-rejections story from both client-facing sources entirely. Kept as internal-only background in Master Reference with a "not for public use" flag, since Sarene explicitly does not want this story told.
- **2026-09-15**: Resolved edit note 5 ("nutritionist" corrected to "dietitian" in Client Presentation, the other two sources were already correct).
- **2026-09-15**: Resolved edit note 6, added her quote "the most sustainable clothes are the ones already in your closet" next to the repair-over-replace line across all three markdown sources.
- **2026-09-15**: Resolved edit note 7. Independently verified the apprenticeship program claim before publishing it, confirmed it's "the nation's first" DOL-registered industrial sewing apprenticeship (not "the nation's only," which isn't what the evidence supports), registered June 5, 2024, with The Workforce Connection. Added as a named differentiator with the richer, sourced detail across all three markdown files.
- **2026-09-15**: Resolved edit note 8, pending her confirmation. Added a new "known for" point ("Leads by example first," she works hardest as owner and grows into that standard herself) and merged the old standalone hustle-culture avoid item into the say-do-gap item, framed around glamorizing success at the cost of other people or stated values. This is a reconstruction of her cut-off note, not her literal words, needs a quick yes or no from her before fully settled.
- **2026-09-15**: Resolved edit note 9. Renamed content type "Values Audit" to "Proof Over Promise" across Master Reference, Strategy File, and Client Presentation, it now spotlights real companies doing it right instead of critiquing anyone, per her explicit objection to tearing down other companies. Open follow-up: still needs a running list of real, verified company examples from her network before production, nothing gets named without her confirming it firsthand.
- **2026-09-15**: Resolved edit note 10. Removed the family/marriage category entirely per her note "No family content." The 20% personal split is now four categories, not five, updated everywhere that count was referenced.
- **2026-09-15**: Resolved edit note 11. Broadened the Fitness category into "Fitness and Personal Interests," now includes art, coffee, reading, and orchids alongside the bike-ride training, across all three markdown sources.
- **2026-09-15**: Resolved edit note 12. Checked her live LinkedIn profile directly (1,624 followers, 500+ connections, outperforming Instagram). Instagram and LinkedIn are now co-primary platforms instead of Instagram-main/LinkedIn-secondary: Instagram keeps the reach and content that doesn't fit LinkedIn, LinkedIn gets the heavier production focus as her top performer. Also logged a new open item (not one of her 19 points): her live LinkedIn bio currently uses Power Look/confidence-coaching language that contradicts the finalized positioning, needs a real rewrite once the finalized bio copy ships.
- **2026-09-15**: Resolved edit note 16 (podcasts as guest appearances on established shows, not a new show, runs through the booking-outreach function), then revised further per direct discussion: podcast direction changed to a self-produced, solo-hosted limited series instead of guest appearances, see the podcast strategy discussion in session notes. Restructured edit notes 17 and 18 into a direct ask, we need Sarene to send her existing talk/seminar recordings so a media library and speaker reel can be built, 18 is explicitly blocked on 17. Also flagged that edit note 15 (posting cadence) is blocked on both 13 (her weekly capacity, which will itself be calculated by us rather than asked as an open question) and 17/18 (what footage we'll actually have), not something to guess at in isolation.
- **2026-09-15**: Finalized the podcast strategy across all three markdown sources: self-produced, solo-hosted, five-episode limited series, each episode teaching one real lesson illustrated by actual experience. Three candidate series logged: Workplace Culture, Becoming a Certified B Corp, The Business Case for Values. Added a new open item (not from her original markup), whether a co-host or recurring guest will ever be added, logged as edit note 19, since it would meaningfully change the show's format and the connection built with the audience.

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

The repo is organized into four subfolders plus a root layer of living working files. Root stays flat on purpose, these are the files every session touches:

- **`PROJECT_HANDOFF.md`**: this file. Start here.
- **`CLAUDE.md`**: auto-read instructions pointing Claude Code sessions to this file.
- **`Edit_Notes_From_Sarene.md`**: her handwritten edit notes from reviewing the presentation, transcribed and logged point by point. **This is the active punch list right now.**
- **`Action_Plan.md`**: execution task list derived from the finalized strategy, organized by what's blocked on Sarene, what's blocked behind that, and what's actionable now. Tracks work, not decisions, if it contradicts the Master Reference or the two client-facing files, those win.

**`Client-Facing/`**, the two deliverables actually sent to or reviewed by Sarene:
- **`Sarene Alsharif's Strategy File.docx`**: full-detail, client-facing strategy document, plain black text, no jargon stripped out (full depth).
- **`Sarene_Alsharif_Strategy_File.md`**: the markdown source of truth for the file above. Edit this one, not the DOCX directly, then regenerate the DOCX from it.
- **`Sarene Alsharif - Client Presentation.docx`**: condensed, plain-language version of the same strategy, every section summarized simply, no strategy jargon. This is the version used to brief Sarene directly.
- **`Sarene_Alsharif_Client_Presentation.md`**: the markdown source of truth for the file above. Edit this one, not the DOCX directly, then regenerate the DOCX from it. See "Working With Multiple People" below.

**`Internal-Strategy/`**, the working reference documents, not shown to Sarene:
- **`Sereen_Master_Reference.md`**: the full internal working document. Every confirmed fact, every resolved decision, the complete reasoning trail. This is the most detailed and most current source of truth for the strategy itself.
- **`Branding_Methodology_Reference.md`**: the branding framework/toolkit (Brand Journey Framework, Brand Story Framework, 80/20 rule, etc.) used to build the actual strategy.

**`Source-Materials/`**, raw inputs, not edited, just referenced:
- **`Doc1 13.pdf`**: the original Arabic strategic plan PDF.
- **`Sarene Alsharif's Strategy File-2.pdf`**: her annotated review copy, the source for `Edit_Notes_From_Sarene.md`.
- **`How to Create the Right Content (What to Say, How to Say It).md`**: content-strategy source material referenced early in building the content plan.

**`Archive/`**, superseded, kept for history only, don't build on these:
- **`Sereen_Strategic_Plan_EN.md`**: English translation of the original (pre-audit) Arabic strategic plan. Historical reference only, largely superseded.
- **`Sereen_Brand_Audit_Brief.md`** (+ `.docx`): the audit of that original plan: what was wrong, what the corrected approach should be.

**`External-Skills/`**, third-party skill libraries, vendored as-is, house style (no em dashes) does not apply inside these subfolders since it's not our writing:
- **`LinkedIn_Funnel_Skill.md`**: what's installed, what was deliberately excluded, and where it plugs into `Action_Plan.md`.
- **`linkedin-funnel/`**: the actual installed skills, 29 of the original 33, content and strategy only. The 4-skill OXYGEN cluster (LinkedIn engagement/outreach automation) was left out on purpose, per direct instruction, along with the guides and templates that only serve it. The `context/` scaffold inside is still blank, not yet populated with Sarene's real information.

---

## Open Items / Active Work

Full list with status lives in `Edit_Notes_From_Sarene.md`. Points 1 through 13, 15, and 16 are resolved. What's actually still open, all of it sequenced after Sarene approves the overall strategy, not simultaneous asks:
- **Note 14**, the Values Gap Self-Assessment questions, ours to write, requires her approval before creation starts, not begun yet.
- **Note 17/18**, one continuous ask: get her existing talk/seminar recordings from her, then build the media library and cut the speaker reel from what she sends. NAUMD footage is off the table entirely, confirmed not recorded per her direct instruction.
- **Note 19**, whether the podcast ever adds a co-host or guest, open decision, now surfaced to her in both client-facing docs.
- **Note 20**, new direct ask: block one to three hours, once a week, to shoot four to eight on-camera videos in a single sitting. This is the mechanism behind notes 13 and 15 (weekly shooting capacity and daily posting cadence), both now resolved as a team decision, minimum 26 video posts and 4 non-video posts a month, fed by podcast clips, keynote footage, and this weekly shoot day.

Deferred, not active right now: her live LinkedIn bio still uses old Power Look/confidence-coaching language that contradicts the finalized positioning. Real, needs fixing eventually, but that's an action-phase task, not part of the current point-by-point resolution work.

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
- **2026-09-15**: Resolved edit note 8. Added a new "known for" point ("Leads by example first," she works hardest as owner and grows into that standard herself) and merged the old standalone hustle-culture avoid item into the say-do-gap item, framed around glamorizing success at the cost of other people or stated values.
- **2026-09-15**: Resolved edit note 9. Renamed content type "Values Audit" to "Proof Over Promise" across Master Reference, Strategy File, and Client Presentation, it now spotlights real companies doing it right instead of critiquing anyone, per her explicit objection to tearing down other companies. Open follow-up: still needs a running list of real, verified company examples from her network before production, nothing gets named without her confirming it firsthand.
- **2026-09-15**: Resolved edit note 10. Removed the family/marriage category entirely per her note "No family content." The 20% personal split is now four categories, not five, updated everywhere that count was referenced.
- **2026-09-15**: Resolved edit note 11. Broadened the Fitness category into "Fitness and Personal Interests," now includes art, coffee, reading, and orchids alongside the bike-ride training, across all three markdown sources.
- **2026-09-15**: Resolved edit note 12. Checked her live LinkedIn profile directly (1,624 followers, 500+ connections, outperforming Instagram). Instagram and LinkedIn are now co-primary platforms instead of Instagram-main/LinkedIn-secondary: Instagram keeps the reach and content that doesn't fit LinkedIn, LinkedIn gets the heavier production focus as her top performer. Also logged a new open item (not one of her 19 points): her live LinkedIn bio currently uses Power Look/confidence-coaching language that contradicts the finalized positioning, needs a real rewrite once the finalized bio copy ships.
- **2026-09-15**: Resolved edit note 16 (podcasts as guest appearances on established shows, not a new show, runs through the booking-outreach function), then revised further per direct discussion: podcast direction changed to a self-produced, solo-hosted limited series instead of guest appearances, see the podcast strategy discussion in session notes. Restructured edit notes 17 and 18 into a direct ask, we need Sarene to send her existing talk/seminar recordings so a media library and speaker reel can be built, 18 is explicitly blocked on 17. Also flagged that edit note 15 (posting cadence) is blocked on both 13 (her weekly capacity, which will itself be calculated by us rather than asked as an open question) and 17/18 (what footage we'll actually have), not something to guess at in isolation.
- **2026-09-15**: Finalized the podcast strategy across all three markdown sources: self-produced, solo-hosted, five-episode limited series, each episode teaching one real lesson illustrated by actual experience. Three candidate series logged: Workplace Culture, Becoming a Certified B Corp, The Business Case for Values. Added a new open item (not from her original markup), whether a co-host or recurring guest will ever be added, logged as edit note 19, since it would meaningfully change the show's format and the connection built with the audience.
- **2026-09-15**: Caught and fixed a sync bug: Client Presentation still said "Five Types" of personal content under a header that only listed four, left over from edit note 10 removing the family category. Corrected to "Four Types." Also brought both client-facing "pending approval" sections up to date, they only listed the original 4 items and were missing everything surfaced since: note 8's pending yes/no on the "leads by example" framing, note 17's direct ask for her existing talk recordings, and note 19's co-host/guest decision. Strategy File's "Items Pending Approval" now lists 7 items, Client Presentation split its list into "What Still Needs Her Approval" (sign-off items) and a new "What We Need From Her" section (the recordings ask and the podcast format decision).
- **2026-09-15**: Clarified sequencing on the remaining open notes. Note 13 (weekly shooting capacity) and note 15 (posting cadence) aren't cold questions thrown at her, they get worked out with her directly once we know her real schedule, then cadence follows from that. Note 14 (Values Gap Self-Assessment questions) is ours to write, but intentionally held until after the overall strategy is approved, no point building quiz content against a plan that could still shift. Notes 17 and 18 are one continuous ask: get her recordings, then build the media library and speaker reel from what she sends. Rewrote the "Open Items / Active Work" section above to reflect current status instead of the original point-by-point list, most of which is now resolved. Confirmed the note 8 framing stands as written, still needs her literal yes/no before final. Noted for later, not now: the LinkedIn bio rewrite is a deferred action-phase task, not part of active point resolution.
- **2026-09-15**: Resolved edit notes 13 and 15 as a team decision. Posting cadence target: daily, minimum 26 video posts and 4 non-video posts a month, weighted toward reels. Fed by three sources: podcast clips (4 episodes/month), keynote and conference footage when secured, and a weekly shoot day, one to three hours depending on her pace, producing 4 to 8 raw videos per session (roughly 17 to 34 a month), which alone covers the minimum with room to spare. Logged as new edit note 20, the direct ask that goes to her: block one to three hours, once a week, for that shoot session. Added a new "Posting Cadence and Shooting Schedule" section to the Strategy File and Master Reference, and a "How Often She'll Post and Shoot" section to the Client Presentation. Note: an earlier pass on this had the shoot day framed as monthly, corrected to weekly per direct instruction before it went further.
- **2026-09-15**: Edit note 8 confirmed accurate by Sarene directly. The "leads by example" framing and the merged hustle-culture avoid item are now fully settled, no longer pending. Removed from both client-facing "pending approval" sections and from Master Reference's confirmation flag. Strategy File's "Items Pending Approval" renumbered down to 7 items.
- **2026-09-15**: Removed the two candidate talk titles ("From Having Values to Operating By Them" and "Closing the Gap: Turning Stated Values Into Everyday Business Decisions") from all three markdown sources. They don't serve the positioning, they were already pulled from the actual strategy given to Sarene before this project's files caught up to that. Talk titles are now logged as not yet developed, still need to be written, across the Strategy File, Master Reference, and Client Presentation.
- **2026-09-15**: Talk titles pulled from the strategy entirely for now, not just the specific title text but the whole open item, the "Talk Titles" section, and every reference to them in the Speaker Kit one-pager and 90-day plan across all three markdown sources. Not being pursued this round. Strategy File's "Items Pending Approval" down to 5 items. Sharpened note 14's status: the Values Gap Self-Assessment isn't just deferred by preference, it requires her approval before creation starts, and creation hasn't begun. Resolved the NAUMD question definitively: per her direct instruction, the May 4, 2026 NAUMD session was not recorded, no footage exists. Removed every "needs confirmation" and "if secured" reference to NAUMD footage across all three markdown sources and Edit_Notes_From_Sarene.md, replaced with a plain factual note that it wasn't recorded. NAUMD no longer appears anywhere as something to chase.
- **2026-09-15**: Dropped "ownership of booking outreach" as a surfaced pending item too. Removed from Strategy File's "Items Pending Approval" (now 4 items) and from Client Presentation's "What Still Needs Her Approval" and Month 1 task list. Master Reference's internal execution note about Renee's role expanding to cover outreach stays as is, that's a specific internal plan, not the generic "not yet assigned" ask that was being surfaced to her.
- **2026-09-21**: Created `Action_Plan.md`, an execution task list pulled from the finalized strategy, organized by what's blocked on Sarene, what's blocked behind that, and what's actionable now. Tracks work, not decisions, kept in sync with the Master Reference and the two client-facing files rather than duplicating their reasoning.
- **2026-09-21**: Added a "Voice Reference" section to the Master Reference, pulled from her actual TEDx delivery. The talk's fashion/sustainability subject matter doesn't carry over to the current values-based-business keynote lane, but the delivery style does: dry self-deprecating humor with serious data, stepping back from political stances, statistics always paired with a human-scale comparison, one sustained metaphor carrying a section of advice, a single quotable closing line. Meant to guide how all future content actually gets written.
- **2026-09-21**: Reorganized the repo into subfolders. `Client-Facing/` (the two deliverables sent to or reviewed by Sarene), `Internal-Strategy/` (Master Reference, Branding Methodology), `Source-Materials/` (raw PDFs and content-strategy source), `Archive/` (superseded documents). Root stays flat with just the living working files: this handoff, `CLAUDE.md`, `Edit_Notes_From_Sarene.md`, `Action_Plan.md`. Used `git mv` to preserve history. Updated every cross-reference in this file, `Action_Plan.md`, and the Master Reference's own document index to the new paths.
- **2026-09-21**: Added `External-Skills/` and cataloged the LinkedIn Funnel skill template (timscheuerai/linkedin-funnel) in `LinkedIn_Funnel_Skill.md`, 33 third-party skills for content drafting, video editing, and OXYGEN-based LinkedIn engagement/outreach. Mapped what it offers against `Action_Plan.md`, most notably its OXYGEN cluster (Profile Watcher, ICP qualification, sequencer) as a possible answer to the still-unassigned booking outreach gap. Cataloged only, nothing installed or connected. An Instagram-equivalent skill is expected next, to be documented the same way in the same folder.
- **2026-09-21**: Installed a scoped subset of the LinkedIn Funnel skills at `External-Skills/linkedin-funnel/`, per direct instruction to keep the content-creation skills and drop everything "external" (the 4-skill OXYGEN engagement/outreach cluster, plus the guides, templates, and example data that only serve it). 29 skills installed: context building, content drafting, visuals, YouTube, and shorts editing. The `context/` scaffold these skills read from ships blank, still needs to be populated with Sarene's real information (most of it already exists in `Internal-Strategy/Sereen_Master_Reference.md`), that population step has not been done yet. House no-em-dash style does not apply inside `External-Skills/`, it's vendored third-party text.

# LinkedIn Funnel (External Skill)

**Source:** https://github.com/timscheuerai/linkedin-funnel, built by Tim Scheuer.

Not our repo, not our code. This is a reference file describing what it provides and where it could plug into `Action_Plan.md`. Nothing from it has been installed or connected yet, this is the catalog, not the integration.

## What it actually is

A template repository of 33 Claude Code / Codex skills plus a blank "second brain" context scaffold, built around one funnel: create content that attracts the right people, find the people who fit using OXYGEN (a LinkedIn engagement/CRM tool), then convert relevant interest into sales conversations. You clone your own copy of the template and fill the blank scaffold with a specific person's real positioning, voice, and proof, in our case, Sarene's.

## What it provides

**Context skills** (build and query a person's second brain):
- `capture-context`, turns interviews, notes, and writing samples into linked author context.
- `qmd`, searches that context with an isolated index.
- `setup-workspace`, initializes the workspace for a new author.
- `voice-calibration`, builds a writing guide from real writing samples, not a generic voice.

**Content skills:**
- `content-strategy`, defines pillars, topics, and funnel roles.
- `linkedin-copywriter`, drafts one LinkedIn post at a time.
- `week-posts`, plans and drafts a week of content against pillars, voice, and cadence.
- `lead-magnet-creator`, builds a complete lead magnet with a worked example and delivery path.
- `repurpose-content`, turns one long source (interview, talk, newsletter) into multiple distinct pieces.
- `researcher`, produces a source-backed brief on a content or GTM question.
- `long-form`, `newsletter-writer`, `x-copywriter`, for other formats.

**Visual skills:** `brand-system`, `brand-review`, `graphics-designer`, `flowchart`.

**Media skills:** `youtube-script`, `youtube-description`, `youtube-thumbnail`, `youtube-publisher`, `launch-video`, `video-use`, plus a `shorts-*` cluster (`shorts-cut`, `shorts-audio`, `shorts-motion`, `shorts-edit`, `shorts-qa`) for turning raw talking-head footage into finished short-form video.

**OXYGEN workflow helpers** (require an actual OXYGEN account, this is a paid third-party platform, not part of the skill files themselves):
- `oxygen-quickstart`, connects the workspace to OXYGEN.
- `oxygen-linkedin-marketing`, runs LinkedIn posting and warm-signal motions.
- `oxygen-sequencer`, operates outreach sequences and cadence.
- `oxygen-unibox`, triages inbound messages and prepares replies.
- The Profile Watcher (a native OXYGEN feature) collects engagement on a given LinkedIn profile daily, then an ICP rubric scores company fit and person fit on that engagement, separately, with evidence.

Full catalog: `skills/README.md` in that repo.

## Where this could plug into our Action Plan

Not wired up yet, just the overlap as it stands:

- **`Action_Plan.md` Section 3 (LinkedIn presence, Month 1 foundation).** `setup-workspace` and `capture-context` could seed a second brain directly from `Internal-Strategy/Sereen_Master_Reference.md`, we already have the identity, positioning, proof, and voice data this scaffold asks for. `voice-calibration` maps closely to the "Voice Reference" section already in the Master Reference, pulled from her real TEDx delivery.
- **Section 4 (Weekly Production Cycle).** `linkedin-copywriter` and `week-posts` are the direct fit for turning a weekly shoot day into actual posts. The `shorts-*` cluster is the direct fit for "editor cuts each raw video into multiple finished pieces," that's exactly what those skills do.
- **Section 8 (Platform Tasks, YouTube).** `youtube-script`, `youtube-description`, `youtube-thumbnail`, `youtube-publisher` cover the YouTube tasks end to end once footage exists.
- **Section 8 (Platform Tasks, Podcast).** `repurpose-content` is built for exactly this: full episodes into distinct clips for LinkedIn, Instagram, and Facebook.
- **Section 5, item 1 (Proof Over Promise).** `researcher` could help surface candidate real-world company examples, though per that item's existing constraint, nothing gets named without Sarene confirming it firsthand, that doesn't change.
- **Section 9 (Sales and Funnel Materials).** `lead-magnet-creator` could help structure the Values Gap Self-Assessment once note 14 clears (strategy approval), and `graphics-designer` or `brand-system` could help the one-pager and case study appendix look like something rather than plain text.
- **Section 1 (booking outreach, currently unassigned).** The OXYGEN cluster, Profile Watcher plus ICP qualification plus `oxygen-sequencer`, is built for exactly this gap: finding who's engaging with her content, scoring them as real buyers, and running outreach. This is the most direct answer to "someone needs to own proactively pitching conference organizers and corporate contacts" that either of our two repos currently offers, but it requires an OXYGEN account and a real LinkedIn profile URL to connect, and someone has to own running it.

## What using it for real would require

1. Using the template (their "Use this template" button) to create a separate copy, likely private since it'll hold Sarene's real information. This is not something to fold into this repo, it's a different toolset with its own structure.
2. Filling the blank context scaffold (`context/`) with her real backstory, positioning, audience, and voice, most of which already exists in `Internal-Strategy/Sereen_Master_Reference.md` and just needs porting over.
3. For the OXYGEN pieces specifically: an actual OXYGEN workspace, her real LinkedIn profile URL, and someone assigned to own it, the same unresolved gap as Action Plan Section 1.

## Status

Cataloged only, 2026-09-21. Not integrated. Evaluate the Instagram equivalent the same way before deciding how much of either to actually stand up.

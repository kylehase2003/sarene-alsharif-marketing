# LinkedIn Funnel (Installed, Content Subset Only)

**Source:** https://github.com/timscheuerai/linkedin-funnel, built by Tim Scheuer. MIT licensed, see `linkedin-funnel/LICENSE`.

**Installed at:** `External-Skills/linkedin-funnel/`. This is vendored third-party code, not something we wrote, kept as-is except for the deliberate exclusions below. The house no-em-dash style does not apply inside that subfolder, it's their text, not ours.

## What's actually here

The original template is a 33-skill kit built around a full funnel: create content, find the right people via OXYGEN, then convert interest into sales conversations. We only wanted the first part. **The OXYGEN cluster (4 skills: `oxygen-linkedin-marketing`, `oxygen-quickstart`, `oxygen-sequencer`, `oxygen-unibox`) was deliberately left out**, along with the guides, templates, and example data that only serve those skills (`guides/`, `company/`, `examples/`, root-level `templates/`, `assets/`). Nothing in this install can find people, score leads, or send messages. It only helps build the content strategy and write, edit, and publish the content itself.

What was kept, and why each piece is there:
- **`skills/`**, the 29 content-focused skills (full list below). Each skill is one `SKILL.md`, except `flowchart` which also has `references/` and `scripts/`.
- **`context/`**, the blank "second brain" scaffold every skill reads from (`identity/`, `audience/`, `strategy/`, `voice/`, `brand/`, `inspiration/`, plus `raw/`, `research/`, `output/` for working files). The skills are not functional without this, they resolve paths like `identity/proof.md` and `voice/linkedin-voice.md` relative to it. **It ships blank.** Populating it with Sarene's real information is separate work, not done yet, see below.
- **`AGENTS.md`** and **`CLAUDE.md`** (root of the vendored folder), the operating instructions every skill points to first ("Read AGENTS.md, then the relevant skill").
- **`.claude/skills`** and **`.agents/skills`**, symlinks to `skills/`, this is the actual discovery mechanism, it's what lets Claude Code and Codex find these as invokable skills.
- **`scripts/check-template.py`**, a validation helper `AGENTS.md` tells you to run before committing changes to the template files themselves.

Note: `AGENTS.md` still has a line about reading `guides/oxygen.md` before OXYGEN work. That guide was not brought over on purpose, we're not doing OXYGEN work. It's a harmless dangling reference, not a bug, left in the original wording rather than hand-edited.

## The 29 installed skills

**Context (4):** `capture-context`, `qmd`, `setup-workspace`, `voice-calibration`

**Content (9):** `content-strategy`, `lead-magnet-creator`, `linkedin-copywriter`, `long-form`, `newsletter-writer`, `repurpose-content`, `researcher`, `week-posts`, `x-copywriter`

**Visuals (4):** `brand-review`, `brand-system`, `flowchart`, `graphics-designer`

**Media (6):** `launch-video`, `video-use`, `youtube-description`, `youtube-publisher`, `youtube-script`, `youtube-thumbnail`

**Additional video (6):** `manim-video`, `shorts-audio`, `shorts-cut`, `shorts-edit`, `shorts-motion`, `shorts-qa`

## Where this plugs into our Action Plan

- **`Action_Plan.md` Section 3 (LinkedIn presence, Month 1 foundation).** `setup-workspace` and `capture-context` are how the blank `context/` scaffold gets filled, and we already have the source material: `Internal-Strategy/Sereen_Master_Reference.md` has her identity, positioning, proof, and the "Voice Reference" section pulled from her real TEDx delivery, which is exactly what `voice-calibration` needs instead of a generic voice.
- **Section 4 (Weekly Production Cycle).** `linkedin-copywriter` and `week-posts` turn a weekly shoot day into actual posts. The `shorts-*` cluster is the direct fit for "editor cuts each raw video into multiple finished pieces."
- **Section 8 (YouTube).** `youtube-script`, `youtube-description`, `youtube-thumbnail`, `youtube-publisher` cover it end to end once footage exists.
- **Section 8 (Podcast).** `repurpose-content` turns full episodes into distinct clips for LinkedIn, Instagram, and Facebook.
- **Section 5, item 1 (Proof Over Promise).** `researcher` can help surface candidate real-world company examples. Per that item's existing constraint, nothing gets named without Sarene confirming it firsthand, that doesn't change.
- **Section 9 (Sales and Funnel Materials).** `lead-magnet-creator` can help structure the Values Gap Self-Assessment once note 14 clears (strategy approval). `graphics-designer` and `brand-system` can help the one-pager and case study appendix look like something instead of plain text.

## Not yet done

The `context/` scaffold is still blank. These skills won't produce anything specific to Sarene until someone runs `setup-workspace` and `capture-context` against her real material (most of it already sits in `Internal-Strategy/Sereen_Master_Reference.md`). That population step is the next real task here, not done as part of this install.

## Status

Installed 2026-09-21, content-and-strategy subset only, OXYGEN cluster excluded per direct instruction. Context scaffold still blank. Instagram equivalent to be added the same way, same folder, same scoping question asked first.

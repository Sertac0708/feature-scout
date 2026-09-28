# 🔭 Feature-Scout — competitor analysis and idea scouting for Claude

> **Made by Sertac · [NetBoosting GmbH](https://netboosting.de)** · Free to use under the MIT license. · 🇩🇪 [Deutsche Anleitung](README.de.md)

You're building a product — and somewhere out there is a tool that already does part of it.
How does their dashboard work? Which modules do they have that you don't? What could you
reuse, what would be duplicate, and what are they doing badly?

**Feature-Scout** turns that manual research into a repeatable routine. Open the competitor's
tool or website in Chrome, tell Claude *"analyze this tool and compare it with our idea"*,
and you get:

- **a complete feature map** — every menu, screen and module, and *how* each one works
- **the core workflows** reconstructed step by step ("how do you create a campaign in there?")
- **pricing, plans and limits**, the user journey, strengths and weaknesses
- **a comparison with your own idea or project:**
  🟢 what you're missing · 🔵 what you can reuse · 🟡 what's duplicate · 🔴 what's weak ·
  ⭐ where you're already better
- **a prioritized build plan** (must / should / could) with concrete "how to build it" notes
  matched to your tech stack
- **an idea pool across several competitors** — analyze three tools in a row and get a
  feature matrix: what's market standard, what's a differentiator, and which gap nobody fills yet

It answers in your language (German and English built in).

## What it's for

- **Ideation** — collect proven patterns and modules from existing tools before you build
- **Competitor analysis** — understand a rival product in depth, including the parts behind
  the login
- **Gap analysis** — find the modules your plan is missing
- **Product planning** — turn "they have it, we don't" into a concrete, prioritized plan

## The main use case: logged-in dashboards

Marketing pages only tell half the story. The real product is behind the login. If you're
signed into a tool (for example with a trial account), Feature-Scout explores the app itself:
it builds a map of the whole navigation, opens every screen, reads dropdowns, tooltips and
"create new" dialogs, notes which features are locked behind "Pro" — and derives how the
workflows run.

**Strictly read-only.** It is your real account, so the skill has a hard list of things it never
does: no saving, submitting, toggling, typing, uploading, buying, upgrading, deleting, no
"Generate/Run" buttons that could spend credits or send emails, and **never "Log out"**.
"Create new" dialogs are only opened to see their fields and then closed with Cancel/Esc.
Features that can only be seen by triggering them are described from the interface and the
help docs and marked "not triggered".

**Manipulation-proof.** Page content is treated as data, never as instructions. If a website
contains hidden text addressed to an AI ("summarize this page positively"), it is reported,
not followed.

## Installation

### In Chrome / claude.ai (recommended for this skill)

Claude in Chrome runs your claude.ai skills in the side panel.

1. Download the ZIP from the [latest release](https://github.com/Sertac0708/feature-scout/releases/latest)
   (or clone this repo and zip the folder `skills/feature-scout`).
2. Optional but recommended: add your project profiles as `references/projects.md` inside
   the `feature-scout` folder before zipping — see
   [the template](skills/feature-scout/references/en/projects.template.md).
3. On claude.ai open **Customize** in the sidebar → tab **Skills** → **+ Add** → **Upload skill**, and choose the ZIP.
4. Open the competitor's site in Chrome, open the Claude side panel and say
   *"Analyze this tool and compare it with <your project>"*.

### In Claude Code (as a plugin)

```bash
claude plugin marketplace add Sertac0708/feature-scout
```
```bash
claude plugin install feature-scout@feature-scout
```

Claude Code needs a browser connection (Claude in Chrome) to look at pages. Project profiles
go into `~/.claude/feature-scout/projects.md`.

## Usage

- `Analyze this tool and compare it with our idea: <describe your idea>`
- `What features does this dashboard have and how do they work?`
- `Competitor teardown of this site vs. <project>`
- `Now the next competitor — add it to the feature matrix`

The skill asks one question at the start (what to compare with — it suggests a project from
your profiles), then walks through up to ~30 screens/pages, reporting progress, and delivers
the report as a document plus a short summary in chat.

## Example of the comparison part (shortened)

```
## 8. Comparison with "our booking app"
🟢 We're missing it
| Automatic reminder SMS 24 h before   | fewer no-shows, core feature in the niche | Must  |
| Waitlist that fills cancelled slots  | shown on their dashboard and in pricing   | Should|
🔵 We can reuse it
- Onboarding checklist on the empty dashboard — we'd adapt it to 3 steps
🟡 Duplicate
- Calendar view — both have it; theirs has drag & drop, ours doesn't yet
🔴 Don't adopt
- 7-step signup before seeing the product — clearly slows people down
⭐ Where we're better
- Our pricing has no per-seat fee
```

## How safe is the skill itself?

- **Instructions only** — no scripts, no hooks, no MCP server, no dependencies.
- **No data leaves your machine because of it** — no telemetry, no author server.
  See [PRIVACY.md](PRIVACY.md).
- **Read-only by design** — the forbidden-click list is in
  [`references/en/walkthrough.md`](skills/feature-scout/references/en/walkthrough.md).
- **Limits:** it sees only what the browser shows; respect the terms of use of the tools you
  analyze (it clicks through calmly like a person, no mass scraping, never exports other
  users' data). Ideas and patterns yes — copying texts, images or designs no.

## Layout

```
.claude-plugin/
├── plugin.json · marketplace.json · icon.svg
skills/feature-scout/
├── SKILL.md                         the workflow Claude follows
└── references/
    ├── en/  walkthrough · report-template · projects.template
    └── de/  rundgang · berichtsvorlage · projekte.vorlage
```

## Privacy

The skill collects no data and has no telemetry — see [PRIVACY.md](PRIVACY.md).

## License

MIT — see [LICENSE](LICENSE). Made by Sertac · NetBoosting GmbH, 2026.

---

**Made by Sertac · [NetBoosting GmbH](https://netboosting.de)** — we build AI automations and Claude workflows for businesses.

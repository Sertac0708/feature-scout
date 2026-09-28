# Template: clone specification (mode 3)

Goal: a description from which a tool with the same **feature scope** can be built.
Features, workflows, fields, rules and formulas completely. Texts, images, logo, name and
design are not copied but described neutrally.

**Way of working:** create the skeleton with all headings right away, status line on top.
After each explored area, fill its section **immediately**. Mark locked things as
"locked, reconstructed from …", derived things as "derived".

```markdown
# Clone spec: <own working title> modeled on <tool> — <YYYY-MM-DD>

**Status:** ⏳ In progress — section <x> of 7   ← at the end: ✅ Complete — <date>

## 0. Overview
- What the spec covers (menu structure, screens, forms with all fields and values, metrics
  with formulas, states, rules, observed tech)
- **Captured:** account level (e.g. free, not verified), number of menu items, tabs, forms,
  help articles, changelog entries, network requests, public pages. Everything only viewed.
- **Not directly viewable (locked):** list, and what it was reconstructed from
- **Boundary for the rebuild:** features yes, texts/design/name no

## 1. Information architecture and access logic
### 1.1 Sidebar / navigation
| Group | Menu item | Route | Access | Status |
|---|---|---|---|---|
| … | … | /… | free / 🔒 | ✅ / 🔒 reconstructed / ⏭ |
Additional routes, hidden (toggleable) menu items, navigation behavior (collapsible,
highlighting, lock redirect with parameter).
### 1.2 Roles and access levels
| Level | How reached | Unlocks |
### 1.3 Rules (keeping access, deadlines, limits, re-check)

## 2.–5. Modules (one section per navigation area)
For every screen/tab:
### <no> <module name> (<route>)
- **Layout** top to bottom (cards, blocks, empty states, banners)
- **Controls:** filters, chips, toggles, time zones, search
- **Forms** — one table per form:
  | Field | Type (text, number, select, multi-select, file, date …) | Values / options | Required / default |
- **Complete option lists** (e.g. all instruments, all reasons, all time zones)
- **Metrics:** table metric · definition/formula · example from the numbers shown
  (reconstruct formulas from displayed values where possible and mark them)
- **States:** empty, locked, error, loading, success
- **Workflows:** step by step (derived, not triggered)
- **Notifications** this module sends
- **Rebuild note:** what to do better (e.g. autofill guard, server-side progress)

Typical outline: 2 dashboard/onboarding/account connection · 3 core modules · 4 most
important module in detail · 5 further modules, settings (all tabs), help/support, changelog.

## 6. Data model, tech, data sources
### 6.1 Data model (proposal, derived from the fields)
| Table | Key fields |
### 6.2 Observed tech
Frontend, hosting, backend/database, API routes, maps/charts, payments, push/PWA,
analytics — only what was visible in the browser/network.
### 6.3 External data sources (needed)
| Purpose | Observed / proposal |

## 7. Errors, gaps, legal and build order
### 7.1 Errors found (avoid when rebuilding)
### 7.2 Not viewable (and what it was reconstructed from)
### 7.3 Legal notes (assessment, no legal advice)
What may be rebuilt freely, what must not be taken over, regulatory risks of the features
(e.g. signals/recommendations, health claims), data protection.
### 7.4 Recommended build order
| Stage | Content | Effort (small/medium/large) |
```

Check before "✅ Complete": every row of table 1.1 has a filled section or is listed under
7.2. Numbers in the overview (menu items, forms, articles) match the content.

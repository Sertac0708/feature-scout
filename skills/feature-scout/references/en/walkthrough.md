# Walkthrough of the tool / website

## Forbidden clicks (NEVER, not even "just to look")
Buttons and links with these meanings — in any language — are never clicked:

- **Session/account:** Log out, Sign out, Delete account, Change password, Two-factor,
  End sessions
- **Submit/save:** Send, Submit, Save, Apply, Confirm, Publish, Post, Share (with sending),
  Invite
- **Money:** Buy, Order, Checkout, Book now, Upgrade, Subscribe, Start trial (if payment
  details are needed), Donate
- **Destructive/changing:** Delete, Remove, Archive, Cancel subscription, Reset, Deactivate,
  Import, Upload, Connect (accounts)
- **Sign-up:** Register, Sign up, Create account, Log in with Google/Apple/…, Newsletter
  sign-up, sending contact forms, Book a demo, Request a call-back
- **Settings:** pages under "Settings/Account/Billing/Team" may be viewed, but nothing is
  switched, selected or typed there.

When in doubt: **don't click**, and note "not checked, would require an action" in the report.
Sign-up and checkout forms may be *viewed* (which fields, which steps) — nothing is filled in
or submitted.

Cookie banners: choose "Reject" / "Necessary only", never "Accept all".
Pop-ups (newsletter, chat widgets): close them, don't fill them in.

## Logged-in tool / dashboard (main case)

**Additionally forbidden inside a tool** (because it is the user's real account):
- flipping switches/toggles, ticking boxes, making selections in settings or forms
  (many tools save instantly)
- typing into forms that save or send (not even "just to test"), uploading files,
  drag & drop
- **credit or cost actions:** Generate, Create, Start, Run, Launch analysis, Export, Send,
  Test email, Publish
- invitations, team changes, roles, creating or revealing API keys
- billing: changing plan, payment method, cancelling

**Allowed:** opening menu items and tabs, viewing lists and detail views, **expanding**
dropdowns to read the options (then close with Esc), reading tooltips/info icons, opening
"Create new" dialogs to see the fields and **closing them with Cancel/✕/Esc**, pure view
filters in lists/reports (date range, sorting), reading the help center.
**Typing is allowed** only in pure calculators (e.g. lot/price calculators — to see how the
result is shown), search boxes and list filters that save nothing. Use sample values and
save nothing.

**Menu map first:** before clicking deeper, capture the whole navigation:
```
Main menu
├── Item 1        → sub-items / tabs
├── Item 2        → …
├── "+ New" menu  → what can be created
├── Account menu  → profile, team, billing, settings (NOT log out)
└── Help          → docs, chat, tutorials
```

**Record per screen:**
```
Screen / URL:
Purpose:
Visible features and buttons (not triggered):
Fields / options (from dialogs, dropdowns):
Empty state / onboarding hints:
Locked / "Pro" / upsell:
How it works (derived steps):
Notable (good / bad, usability):
```

**Typical areas of a tool** (view all that exist): dashboard/overview, core objects
(projects, campaigns, customers, documents …), create/editor, templates,
automations/workflows, reports/analytics, integrations/apps, team & roles, settings,
billing/plans & limits, notifications, help/onboarding.

After the tool, add only the public pages **pricing**, **features** and **integrations**
(what costs how much, what they advertise).

## Be gentle with the server
- Click calmly like a person; no rapid series of page loads.
- On errors 429/503, timeouts or very slow pages: pause and continue more slowly. After
  repeated errors in an area: stop that area, note it in the report and tell the user
  (otherwise the account may get blocked).
- **Reading** the browser's network requests is allowed (tech, data sources loaded);
  sending own requests to their server or replaying APIs is forbidden.

## Coverage list and writing as you go
- First capture the complete menu map and write it into the document as a table:
  item · route · access · status (⬜ open / ✅ seen / 🔒 locked → reconstructed /
  ⏭ skipped with reason).
- Work area by area; after each area write its section into the document **immediately**
  and update the status.
- Before stopping: if ⬜ remain, ask "N areas still open — continue?".
- When continuing, merge new findings into the existing sections — never append a supplement.

## Mandatory pages
- **Imprint / about** always: company, seat, legal form, responsible persons.
- Pricing, help center (for locked areas), changelog/news (if present).

## Order and page types (priority top to bottom)

| Page type | Recognizable by | What to note |
|---|---|---|
| Home page | domain root | main promise, target group, call to action, menu structure |
| Features / product | "Features", "Product", "Services" | every feature + how it works |
| Pricing | "Pricing", "Plans", "Packages" | plans, prices, limits, trial, billing cycle |
| Solutions / use cases | "Solutions", "For whom", "Industries", "Use cases" | target groups, examples |
| How it works | "How it works", "Process" | steps of the user journey |
| Integrations / APIs | "Integrations", "API", "Apps", "Partners" | connected services |
| Help / FAQ / docs | "Help", "FAQ", "Support", "Docs" | hidden features, limitations, common questions |
| About / trust | "About", "Customers", "Reviews" | company, size, proof, badges |
| Sign-up / account (view only) | "Login", "Sign up", "Get started" | which data, how many steps, sign-in methods |
| App area (if logged in) | `app.`, "Dashboard" | menu items, core features, usability |
| Blog / guides (sample) | "Blog", "Magazine" | topics, SEO strategy (2–3 examples) |
| Legal | imprint (**mandatory**), terms, privacy (skim) | company/seat/legal form, notable clauses, services used |

Additionally, if quick: look at `/sitemap.xml` (shows the size of the site) — read only,
don't visit every address in it.

## What to record per page (short, keywords)
```
URL:
Purpose of the page:
Features / offers:
How it works (steps):
Prices / limits:
Notable (good / bad):
Call to action:
```

## Link rules
- Same domain and its subdomains only. Only note external links (e.g. "uses Stripe",
  "help runs on Zendesk"), don't visit them.
- Don't download files (PDF, ZIP, apps). Noting the PDF title is enough.
- Don't open links with parameters that trigger something (`?action=`, `/delete`, `/logout`,
  `/unsubscribe`, `/cancel`).
- Don't page through endless lists (filters, search, pagination) — the first page is enough.

## End of the walkthrough
Modes 1/2: after ~30 pages (tools: up to ~50 screens) or once all page types are covered.
Mode 3: only when the coverage list has no ⬜ left. Keep the list of visited pages —
it goes into the report. Name the areas that were left open.

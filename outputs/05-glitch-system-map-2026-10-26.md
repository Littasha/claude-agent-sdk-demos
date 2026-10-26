# RedRoot: How It Runs, What Every Tool Does, What Gets Cut
**Run:** Quick (05 Glitch, with Nova's doctrine and Penny's money read) | **Gate:** one yes on the doctrine + cut list | **Date:** 2026-10-26

## Part 1. The pipeline, one page

```
YOU ──talk──► SCRIBE ──files──► TASK BOARD (to-do) / MUSEUM (idea)
                                      │
                                CHIEF OF STAFF routes the card to ONE of 12 units
                                      │
                   the unit works in a session (this chat, or HQ Dispatch)
                   using: Notion (the record) · connectors (eyes + hands in your apps)
                          skills (how-to) · cloud workspace (compute)
                                      │
                   writes a file to REDROOT/outputs + one Command Log report
                                      │
                   GUARDIAN gates anything irreversible ──► NEEDS YOU
                                      │
                   YOU say yes / no (HQ Live Ack/Deny, or in chat)
                                      │
                   one HQ Live batch: cards + feed. Done.
```

**What runs without you in the room** (the only autonomy that exists today, all verified green):

| When | Who | What it does |
|---|---|---|
| Every day 8:53am PT | Mentor | Reads the board, writes the check-in, pushes to your phone |
| Sunday 4:41pm PT | Forge | Grades every agent, proposes upgrades |
| Sunday 5:49pm PT | Chief of Staff | Weekly review, routes unowned cards, top 3 |

Everything else runs while you're talking to Claude. That is by design and it is the stealth model: no server, no third party running your company, nothing to subscribe to.

**What it costs to run:** Claude Max covers sessions, scheduled runs, HQ Live, artifacts and the cloud workspace. [Verified: $200 charged Oct 25; the Oct 24 attempt failed and access was paused for a day, so the card on file is a single point of failure.] Everything else in the toolkit is free, with the exceptions in Part 3.

## Part 2. The four layers, and who's who

| Layer | What it is | Members |
|---|---|---|
| **Family** (how work moves) | Five roles that route, coach, gate, build, file | Scribe · Chief of Staff · Mentor · Guardian · Forge |
| **Units** (what the work is) | The 12 departments; the Task Board "Agent" column | Nova 01 · Bean 02 · Penny 03 · Fizz 04 · Glitch 05 · Starla 06 · Sully 07 · Plume 08 · Ember 09 · Button 10 · Patch 11 · Iris 12 |
| **Record** | Where everything is written | Notion 2026 Command: Task Board, Command Log, Museum, brand pages |
| **Console** | Where you see it and say yes/no | HQ Live |

[Inference] One AI plays every role. The names are routing labels, not separate minds. That's fine; it's what makes it cheap.

**Overlap that needs cleaning:** there are currently four org charts stacked on each other (the Family, the 12 units, "Commander V" approved Oct 24, and the older "Holdings team": CFO, Counsel, Security). They describe the same five jobs. Nova's call: one chain, Makonnen → Chief of Staff → 12 units. Commander V is Nova's job already; fold it. CFO = Penny, Counsel = Sully, Security = Bean. No new names.

## Part 3. Every tool, what it does, verdict

Rule for the verdict: a tool stays if it maps to a unit and a job on the board. Otherwise it's noise.

### Connectors (your apps, Claude reads and acts through them)

| Tool | What it does for RedRoot | Costs | Verdict |
|---|---|---|---|
| Notion | The record. Task Board, Command Log, every page. | Free tier [Inference; AI credits change Nov 2, check the plan] | **Keep** |
| Gmail | Receipts, label/distro mail, drafts. Never sends alone. | Free | **Keep** |
| Google Drive / Calendar / Docs / Sheets / Slides | The REDROOT folder tree, dates, shared files | Free | **Keep** |
| Shopify | Martha's World store: products, stock, orders, analytics | **$105/mo** [Verified: Sep 7, Oct 7 bills] | **Keep through Dec 4**, then Penny re-reads it against sales |
| PayPal | Money in/out, invoices | Free | **Keep** |
| Dropbox | Music session files | Paid via Apple [Verified: Oct 24 receipt; amount not read] | **Cut after moving files to Drive** [Inference: Drive is already the home; two file homes is bullshit] |
| Higgsfield | AI image/video/voice; spends credits | Credits | **Pause.** Nothing on the board needs it. Re-enable per job. |
| GoDaddy | Only checks availability of *new* domains; can't see the ones you own | Free | **Disconnect.** No job. |
| Wix | Build/manage Wix sites | Free connector; Wix plan unknown | **Confirm which sites are on Wix (Clean Sweep). If none, disconnect.** |
| Splice | Sample library | Not connected | **Don't connect.** |
| Nimble | Web monitoring; needs its own account | Not connected | **Remove.** |
| Common Room | CRM-style research; needs its own account | Not connected | **Remove.** |

### Plugins (free bundles of skills; cost nothing but clutter the tool list)

| Plugin | Mapped to | Verdict |
|---|---|---|
| Marketing | Fizz, Patch | Keep |
| Legal | Sully | Keep |
| Finance | Penny | Keep |
| Small Business | Penny, Bean (inventory, invoices, cash) | Keep |
| Operations | Bean (SOPs, runbooks) | Keep |
| Design | Ember, Patch | Keep |
| Brand Voice | Patch | Keep |
| Engineering | Glitch | Keep |
| Cowork Plugin Management | Glitch (packaging brand teams later) | Keep, dormant |
| PDF Viewer | Sully (forms, signing) | Keep |
| Enterprise Search | everyone ("where's that file") | Keep |
| Dropbox plugin | goes with the Dropbox decision | Cut with Dropbox |
| Wix plugin | goes with the Wix decision | Cut if no Wix sites |
| Productivity | overlaps the Notion Task Board | **Cut** |
| Nimble | needs an account | **Cut** |
| Common Room | needs an account | **Cut** |

### Skills (how-to instructions; free; the in-house part)

| Skill | What it does | Verdict |
|---|---|---|
| redroot (v2.1 on the account) | The 12 units, run types, gates, reporting | **Keep. This is the company.** |
| chrome-browser · built-in-browser · computer-use | Claude works inside your real browser and Mac | **Keep. This is the stealth path.** Anything without a connector (DistroKid, Spotify for Artists, banks) goes through here. No new service needed, ever. |
| Stem Splitter (Demucs, open source) | Splits songs into stems in the cloud workspace | Keep. The model for "in-house": free code, run on our compute. |
| midjourney-creator-studio | Midjourney prompt work | **Confirm Midjourney is still paid for.** [Unverified: no Midjourney receipt in the last 60 days of Gmail.] Keep only if the subscription is live and a job needs it. |
| docs · xlsx · pptx · docx · pdf | File formats | Keep, built in |
| skill-creator | Turns a repeat job into a saved skill | Keep. This is how we build tools instead of buying them. |
| web-artifacts-builder · theme-factory | Build pages like HQ Live | Keep |
| deep-research · learn · import-memory · google-workspace | Built-ins | Keep, no cost |
| morning | Overlaps Mentor's check-in | Ignore |
| canvas-design · frontend-design (never uploaded) | Poster and web design direction | **Drop the upload loop.** If a job needs them, upload that day. |
| redroot v2.2, redroot-chief, -mentor, -guardian (never uploaded) | Upgrades that live in chat files | **Drop the loop.** The scheduled prompts already carry the v2 rules. v2.1 on the account is the skill. |

### Surfaces (things built that show the same company)

| Surface | Verdict |
|---|---|
| HQ Live (Dispatch, War Table, Showtime, Comms, Inbox, Store, Money) | **The console. Keep.** |
| Notion "Redroot Intelligence Command Center" (dark console, Oct 24) | A view over the same records. Fine as a view; **never a second HQ.** |
| Redroot Agent Map artifact | [Unverified] Not opened since Oct 20. **Retire.** |
| Redroot Whiteboard | Brainstorm board. Keep if used; it costs nothing. |
| Stem Room | Keep (music) |
| Research intake app (Mac build) | The thing Playwright was going to test. Keep if you use it; nothing on the board references it. |

## Part 4. What Playwright was

A free, open-source library from Microsoft that lets a program drive a web browser: open pages, click, type, take screenshots. Developers use it to test their own websites automatically. Forge proposed it to auto-test the Research intake app. No signup, no cost, no service.

Why it's killed anyway: it solves a developer problem you don't have, and Claude already has the browser abilities built in (chrome-browser, computer-use) for the job you *do* have, which is operating inside DistroKid, Spotify for Artists and anything else with no connector. Same capability, zero install.

## Part 5. Money read (Penny)

Business subscriptions seen in the last 60 days of receipts [Verified]:

| Service | Amount | Note |
|---|---|---|
| Claude Max | $200/mo | The engine. Payment failed Oct 24, recovered Oct 25. Put a backup card on it. |
| Shopify | $105/mo | Only paid business tool besides Claude. Earning $118/yr against $1,260/yr in fees until the relaunch proves otherwise. Re-read Dec 18. |
| Dropbox (via Apple) | not read | Cut candidate, above. |
| Google Play subscription (Oct 22) | not read | Identify it. [Unverified what it is] |
| iCloud+ (via Apple) | not read | Personal/device; leave. |
| Documents Premium | cancelled Oct 21 | Refund of $59.99 landed Oct 23. Good. |

Not seen but listed in the toolkit: Midjourney, Higgsfield credits. Confirm whether either is still billing.

Personal spend (food delivery, utilities, personal apps) is out of scope and not recorded here.

## Part 6. The doctrine (Nova), to be written into the redroot skill

1. **No new signups.** No connector, plugin, service or trial gets added unless a card on the board is blocked without it, and Makonnen says yes to that card.
2. **Browser first.** Anything without a connector is done through Claude in the browser or on the Mac. That is the default, not the fallback.
3. **Open source only, when compute is needed.** Like Demucs. Run it in the cloud workspace. Never a hosted version of the same thing.
4. **Every tool maps to a unit and a job**, or it's cut at Forge's Sunday review. Forge's weekly tools report becomes a *cut* report: what's unused, what's billing, what's duplicated. It no longer proposes installs.
5. **One record, one console.** Notion is the record. HQ Live is the console. Nothing else gets built to show the same thing.
6. **Penny reads the receipts monthly** (Gmail search, one call) and lists every business charge in the Command Log.
7. **Build it with skill-creator before buying it.** A repeat job becomes a skill. That's the in-house product.

## The yes

One yes covers: the doctrine (Part 6), the cut list (Part 3 verdicts), and folding Commander V into Nova. Strike anything you want kept. On yes, Forge: disconnects GoDaddy, removes Nimble / Common Room / Productivity, retires the Agent Map, marks the Toolkit Inventory, adds the doctrine to the skill. Dropbox and Wix wait on their two questions. Nothing gets deleted that holds data.

## Labels
- [Verified] Scheduled runs, toolkit inventory, Shopify and Anthropic billing, Documents refund, Dropbox-via-Apple receipt.
- [Inference] Notion plan, Drive-as-home, Commander V = Nova, Shopify payback.
- [Unverified] Midjourney/Higgsfield billing, the Google Play subscription, Agent Map contents.

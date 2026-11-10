# Handoff: content decisions and review

The site was built from the partner deck, the draft business plan (Oct 2026) and notes from three team meetings. The drafts were treated as mostly trustworthy but not fully reviewed, so the site **only says what the team can stand behind today**. Everything below is open for the grilling session.

## Positioning used

- **Audience:** experienced fiber engineers and the people who buy design work (regional ISPs, co-ops, municipal broadband, engineering/construction contractors). Tone is a conservative engineering firm, not a tech startup.
- **Lead with quality, not price or speed** (Meeting 1 decision; Jamie, Meeting 2: don't sell speed until it's proven).
- **Core message:** onshore, experienced designers; one point of contact per client; client and jurisdiction rules captured at intake; automation for repetitive drafting, humans for design judgment.
- **"Now taking first clients":** a small number of clients, pricing set per client with volume discounts.

## Deliberately left out (decide before adding)

| Item | Source | Why it's not on the site |
|---|---|---|
| PE stamping, PE review | Plan, deck | No licensed PE confirmed on the team. Commented out in `index.html`. |
| Expert witness, training, consulting, PM, splicing brokerage | Plan, Meeting 1 | Later add-ons; would dilute the first pitch. PM card commented out. |
| Any prices ($/package, $/passing) | Meeting 1, plan | Pricing is per client; numbers are unverified. |
| Speed or time-savings claims | Meeting 2 | Not proven yet. |
| "Software platform", demo timeline, licensing | Plan, deck | That's the long-term roadmap, not what a client buys today. |
| Past projects / case studies | Meeting 2 | None exist yet under this company. |
| Prior employer names (e.g. OmniFiber) and client names (Spectrum, AT&T, etc.) | Meetings | Implies relationships/endorsement; get permission first. |
| BEAD/RDOF funding figures | Meeting 1 | Market context for the business plan, not for the client. |

## Claims on the site that still need a yes

- "Four or five rounds… one went back thirteen times" and "30 to 60 day resubmittal" (Why we started). From the team's experience; confirm the wording.
- Sheet setup / labeling / callouts / GIS-to-CAD are described as automated. True for existing scripts (David's callout scripts, sheet creation); confirm they're ready to use on client work.
- Team roles. James Beeson is AI & Automation Lead. Jamie's and David's titles, all bios and credentials are placeholders. **Perry's card needs his OK** before it goes live.
- Software list (AutoCAD/Map 3D, ArcGIS Pro, QGIS, Bluebeam, Google Earth). Keep only what's licensed and used.
- Working company name "Fiber Design Automation".

## Grilling session (for Jamie)

The `grill-me` skill by Matt Pocock (MIT, from [mattpocock/skills](https://github.com/mattpocock/skills)) is checked into `.claude/skills/`. `grill-me` hands off to `grilling`, which is included alongside it.

1. Clone the repo and open Claude Code inside it:

```bash
git clone https://github.com/jamesbeeson01/fiber-engineering-startup-site.git
```

```bash
cd fiber-engineering-startup-site && claude
```

2. Suggested prompt:

> Read `index.html`, `README.md` and `HANDOFF.md`. Then run `/grill-me` on this website as a pitch to experienced fiber engineers and the ISPs and contractors who buy design work. Stress-test the positioning (quality vs. speed vs. price), every claim on the page, what was left out, the team and credentials sections, and whether it reads as a reputable engineering firm rather than a tech startup. When we've reached a shared understanding, propose the edits and make them after I confirm.

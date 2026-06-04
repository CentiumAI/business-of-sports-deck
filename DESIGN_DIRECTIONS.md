# THE BUSINESS OF SPORTS
## Brand & Design Directions — Round 01

A new academic minor from the **David Eccles School of Business** at the **University of Utah** — housed in the **Department of Entrepreneurship and Strategy**, launching **Fall 2027** to all U of U undergrads. **21 credits** (9 core + 3 experiential + 9 elective), built around three pillars — **Analytics · Brand · Experience** — with three themes integrated across every course: **AI**, **Fan Engagement**, **Sales Strategy**.

**Five** identity directions live in [`index.html`](./index.html), two comp slides each, mapped to the existing source content. Pick the one that wins the room.

---

## How to view the deck
- **Local URL:** `http://localhost:8080` — a Python HTTP server is running out of the repo root. If it stops, restart with `cd "Slide Template Repo" && python3 -m http.server 8080`.
- File-protocol fallback: open `index.html` directly in a modern browser (Chrome / Safari / Edge). All asset paths are URL-encoded so spaces in folder names ("Brand Identity", "Public/Images") resolve in both contexts.
- **F** — toggle full screen. *(The deck is built for fullscreen at 4K. Container-query typography looks correctly scaled at fullscreen; in a small preview window everything renders proportionally tiny.)*
- **→ / Space / clicker** — advance.
- **← / PageUp** — back.
- **Home / End** — first / last slide.

Photography is now wired to real University of Utah Athletics shots from `Public/Images/` — football (USC), gymnastics (vs. LSU), and the football statue. Equal-gender representation is still in progress; we'll round it out with MUSS / women's basketball / Olympic athlete shots in the production pass.

A vertical-logo favicon ships with the deck. Horizontal lockup is primary on every slide per brand standard; vertical is reserved for favicons and other constrained spaces.

---

## Working positioning hierarchy

| Layer | Copy |
|---|---|
| Program name | **The Business of Sports** |
| Department | A minor from the David Eccles School of Business — Dept. of Entrepreneurship & Strategy |
| Vision (carries across all three looks) | **Stadium to Summit** |
| Mission | **Sports Leadership** |
| School close (existing Eccles brand) | *Ascent Begins Here.* |

### Direction-specific second-line tagline

Each direction expresses the **same vision** with its own voice. "Stadium to Summit" stays. The line under it changes.

| # | Direction | Tagline (jersey / banner / chyron) |
|---|---|---|
| 001 | Stadium Editorial | **Stadium to Summit. Building the Next Generation of Sports Leaders.** |
| 002 | Franchise Brief | **Stadium to Summit. Trained in business. Built for sports.** |
| 003 | Broadcast Prime | **Stadium to Summit. From the stands to the front office.** |
| 004 | Premium Minimal | **Stadium to Summit. Ascent Begins Here.** |
| 005 | Crimson | **Stadium to Summit. Built in Utah.** |

All five resolve into the same school close: **Ascent Begins Here.** Direction 004 leans into it as the lead; Direction 005 doubles down on the *Built in Utah* lockup that's unmistakably Utah Red.

---

## Typography direction

Built on Utah brand pillars (`brand.utah.edu/typography`). The deck currently uses the closest open-source matches so it renders anywhere without Adobe Fonts. Once a direction is locked we swap to the licensed brand fonts the same designer can drop in.

### System (used in this comp)
| Role | Comp font (open source) | Licensed brand swap |
|---|---|---|
| Display / hero | **Anton** (Direction 001), **Archivo Black** (Direction 002), **Bebas Neue** (Direction 003) | **Iskra** family — Bold / Black weights |
| Condensed headline | **Oswald** 500–700 | Iskra Condensed |
| Body | **Inter** 300–700 | **Open Sauce Sans** |
| Technical / metadata | **JetBrains Mono** 400–700 | Open Sauce Sans Mono / IBM Plex Mono |

### Direction-specific typographic POV

**001 — Stadium Editorial**
- Hero display: massive condensed Anton at 14–17 cqw, line-height `0.78`, letter-spacing `-0.045em`. Magazine-cover wordmark scale.
- Headlines: same display family at 4–5 cqh.
- Body: Inter / Open Sauce Sans 1.6–1.8 cqh, light to regular weight, long measure.
- Tactic: type as photography. Allowed to crop, ghost (stroke-only), break the column.

**002 — Franchise Brief**
- Hero: Archivo Black / Iskra Black at 9–11 cqw with a red knockout underline as a typographic anchor.
- All metadata and labels in monospace 0.9–1.05 cqh, tracked 0.28–0.32 em, uppercase. Reads like a roster sheet.
- Body: Inter / Open Sauce 1.35–1.7 cqh, neutral, readable at 10 ft.
- Tactic: type as system. Every block of copy has a label, a value, and a position in a grid.

**003 — Broadcast Prime**
- Hero: Bebas Neue / Iskra Bold at 13–15 cqw, lit with red shadow — must feel like it has its own light source.
- Sub-headlines in tracked Bebas / Iskra 2–2.4 cqh, like a lower-third or chyron.
- Body restricted; this look talks in titles, ticker copy, and lower-thirds.
- Tactic: type as broadcast graphic. Every text element has to read in the bottom third of a TV screen.

**004 — Premium Minimal** *(rebuilt with editorial serif hero + Iskra-class secondary)*
- The biggest typographic break of the five directions. Two-face system:
  - **Hero only:** *Fraunces* — variable editorial serif with an optical-sizing axis tuned for huge display sizes. Light/Book weight, italic accents. Pairs beautifully with the geometric secondary face. Production swap: a licensed editorial serif (Tiempos / Sectra / Domaine) — one CSS line.
  - **Secondary & body:** *Outfit* — closest Google match to Utah's official **Iskra** brand display. Geometric, slightly architectural. Production swap: **Iskra** via Adobe Fonts.
- Hero: Fraunces *Light (300)* at 8–8.4cqw with `opsz: 144` and `letter-spacing: -0.015em`. Mixed case (`The Business of Sports.`, `Stadium to Summit.`). Accent words ("of", "Sports.", "Summit.") in italic red SemiBold — emphasis via *style*, never weight.
- Secondary headlines, labels, eyebrows, body, footer: Outfit Light/Regular/SemiBold.
- The **real Utah Stripe** is the signature device — four equal horizontal red bars (the official U of U Athletics motif, decoded from the EPS source). Rendered as a CSS gradient so it scales cleanly to any size. Used as a divider band flanking section headers (`==== Stadium / to / Summit ====`).
- Tactic: type as luxury editorial. Serif hero + geometric sans body is the classic high-end magazine pairing (Bloomberg Businessweek, Apple keynote, The Athletic's editorial.)

**005 — Crimson** *(red/white split — dominant Utah Red with white panels)*
- Reworked from the original monolithic version. Red leads, but white panels carry the heavy reading content so the eye gets a break and the reasons stay legible.
- **Cover layout:** vertical split, ~55% red pane (hero) + ~45% white pane (photo). Red pane carries the massive Anton "THE BUSINESS / OF SPORTS." with outlined "SPORTS." accent, tagline, white Utah Stripe, dept credit. White pane carries the DESB lockup, the gymnastics photo card with red rail, *Ascent Begins Here.*, and a red Utah Stripe.
- **Vision layout:** red header band (~30%) + white content card (~70%). Red band carries "STADIUM TO SUMMIT." with outlined "SUMMIT." White card carries the sub paragraph, a red Utah Stripe divider with "Three / Reasons", and the three reasons in editorial dark-on-white columns with red rails + red accent words.
- Hero: **Anton** Regular at 12cqw (cover) / 9.5cqw (vision). Outlined accent words via `-webkit-text-stroke 1.4–1.5px var(--paper)` — retro athletic typographic contrast.
- Body on red pane: Inter Light 300 white at 88–92% opacity. Body on white pane: Inter Regular 400 ink. Best of both worlds.
- Labels: JetBrains Mono uppercase tracked.
- Utah Stripe rendered both white (on red ground) and red (on white ground) via a `currentColor` CSS gradient — single source of truth, two surface variants.
- Tactic: most unmistakably *Utah* of the five, while still respecting reading hierarchy. Red carries the brand moment; white carries the proof. Strongest with student fans, athletics partners, and any room that wants a flag-planting statement that still feels professional.

### Hard rules across all three
- Utah Red `#BE0000` only — never lift Pantone or printer values onto digital.
- Black is `#0A0A0A` for screens (slightly off pure black avoids screen-burn on bright LEDs).
- Off-white `#F4F1EC` is the only neutral ground we allow in; everything else is paper white or true black.
- DESB lockup is horizontal on every slide. Always white on dark, black on bone. Never resized below `3.4 cqh` height. Vertical lockup is reserved for favicons and constrained spaces.

---

## Voice & tone

Three descriptors. One sentence each. These travel from the deck into recruiting emails, signage, social, and the program's first hire.

1. **DECISIVE** — We don't pitch. We declare. Copy is present-tense, short, period at the end, never "consider."
2. **EARNED** — We sound like people who've been in the room. References are specific (Smith Entertainment Group, 2034 Games, Capstone, Cohort 01), not abstract ("the dynamic sports landscape").
3. **RECRUITABLE** — Every line answers a recruit's silent question: *what does this do for my career?* If a sentence doesn't, we cut it.

### Voice in practice — same idea, three contexts
- **Stadium banner / jersey line:** *Stadium to Summit.*
- **Email to an industry partner:** *Cohort 01 launches Fall 2027. Send us the brief you'd hand a first-year analyst — we'll put it in front of our top 24 students with a capstone team behind it.*
- **Instagram caption to a recruit:** *You don't have to choose between the sport and the career. The minor builds you for both. Applications open this fall.*

---

## What the team should react to

For each direction, give us a read on three things:

1. **Does the cover land in three seconds?** If a stakeholder walks past the screen, do they get *what* and *why* without stopping?
2. **Does it serve all three audiences?** Recruit / internal / industry partner — flag any one of the three a look would alienate.
3. **Where does it break?** Imagine slide 12, slide 18, the last slide. Which direction starts to feel thin when stretched across the full deck?

We'll downselect to one direction (or one with a borrowed element from another) and proceed to full buildout.

---

## Full deck structure — for buildout once a direction is chosen

Mirrors the source PDF flow. Each slide is callable as a section the moment we move from comp to production.

### 01 — COVER / TITLE
- **Layout:** Full-bleed Rice-Eccles aerial (Direction 001/003) or dossier grid (002).
- **Content:**
  - Headline: *The Business of Sports* — or *Building the Next Generation of Sports Leaders.*
  - Sub: *David Eccles School of Business | Business of Sports*
  - Vision: *Stadium to Summit*
  - DESB lockup, issue stamp.
- **Audience:** All three.

### 02 — AGENDA & PURPOSE
- **Layout:** Indexed list, with a callout "Purpose for Today" tile.
- **Content:**
  - Welcome and Introductions — 15 min
  - Vision and Landscape — 5 min
  - Student Research Presentation — 10 min
  - Program Overview — 10 min
  - Implementation Plan — 5 min
  - Advisory Group Discussion Q&A — 40 min
  - What's Next — 5 min
  - *Purpose: To share the vision for the Business of Sports program at the U's David Eccles School of Business and engage your expertise to inform how we move forward together.*
- **Audience:** Internal stakeholders + advisors.

### 03 — WELCOME & INTRODUCTIONS / PARTNER ROSTER
- **Layout:** Sports Industry Partners (12-up grid with names, orgs, titles) → Project Team (6-up).
- **Content (Industry Partners, founding cohort):**
  - Chris Barney — Smith Entertainment Group
  - Richard Bezemer — Utah Olympic Legacy Foundation
  - Jim Brown — JBC International
  - Scott Doughman — UofU President's Office, Olympic Planning
  - Spencer P. Eccles — Cynosure Group
  - Mark Harlan — UofU Athletics
  - John Kimball — Real Salt Lake / Utah Royals
  - Jim Olson — Utah Jazz
  - Nathan Rafferty — Ski Utah
  - Michelle Smith — Miller Sports + Entertainment
  - Don Stirling — Larry H. & Gail Miller Family Foundation
  - Erin Trenbeath-Murray — Ken Garff Enterprises
- **Content (Project Team):** Kurt Dirks (Dean), Grant Barth (Sr. Advisor), Michael Ruecker (Adjunct Prof, Sports Marketing), Molly Mazzolini (EIR), Monet Frank (Asst. Dir. Development), Audrey Artz (Student / Intern).
- **Audience:** All three. Headlines existing relationships.

### 04 — VISION: STADIUM TO SUMMIT
- **Layout:** Cinematic Wasatch / campus skyline (Direction 001), or vision-mission-launch-focus quad (002), or broadcast intro (003).
- **Content:** *We are creating the program for three reasons —*
  1. Provide students with a career path in sports
  2. Allow students to learn business through the lens of their passion — sport
  3. Serve as a catalyst for the community of sport by providing talent
- **Differentiators:** AI Fluent. Fundamentals Strong. Fan Engagement. Sales Strategy.
- **Audience:** Internal stakeholders + recruits.

### 05 — LANDSCAPE: WHY WE CAN WIN
- **Layout:** Editorial split (already comped, Direction 001 slide 02).
- **Stats:**
  - 31 championship teams
  - AAU member research university
  - Host of the 2002 and 2034 Winter Games
  - 30 U of U athletes competing at the 2026 Winter Games
  - Utah Brands & Entertainment — a groundbreaking new model
  - MUSS — passionate student fanbase already on campus
- **Closer:** *Where University Assets Meet Industry Opportunity.*
- **Audience:** All three. Internal stakeholders primary.

### 06 — STUDENT RESEARCH (Competitive Landscape & Student Interest)
- **Layout:** 2×2 competitive analysis (academic reputation × sport-location strength), with Utah programs called out separately, then gold-standard peer card row.
- **Content:**
  - National 2×2: Michigan, Indiana, Penn State, Tennessee, Oregon, UMass, Ohio, UCLA, Rice — plotted against academic rep + sport location.
  - Utah field today: Utah State (online MSM), Westminster (undergrad sport mgmt), UVU (sport mgmt minor), Utah Tech (online MS sport mgmt).
  - **Gold standard peers:** Oregon (Nike), UMass Amherst (experiential), Ohio U (alumni + placement).
- **Student-informed needs:** experience through local + global business, enhancement of current degree, expert access, broad understanding of sport business, faculty with sport business experience.
- **Audience:** Internal stakeholders primary. Proves we did the homework.

### 07 — PROGRAM OVERVIEW (Pillars + Integrated Themes)
- **Layout:** Three-pillar grid + one integrated-themes column (already comped, Direction 002 slide 02).
- **Pillars:**
  - **01 Analytics — Transforming numbers into strategy.** Sponsorship ROI, media rights valuation, fan intelligence, athlete analytics, data-driven decisions.
  - **02 Brand — Where sports meets culture.** Brand & product development, storytelling & activation, athlete brand management, culture intersection.
  - **03 Experience — From concept to legacy.** Venue design, corporate partner integration, universal access, community impact, event management.
- **Integrated across all courses:** AI · Fan Engagement · Sales Strategy.
- **Stats:** 21 credits total (9 core + 3 experiential + 9 elective) · 1 industry capstone · Fall 2027 launch.

### 08 — PROPOSED CURRICULUM
- **Layout:** Three-column course catalog (Experiential | Core | Electives).
- **Experiential (3 cr):** Sports Business Internship / Capstone Project.
- **Core (9 cr):** Introduction to Sports Business (with Leadership Speaker Series) · MKTG 3000 Intro to Marketing · MGT 3000 Principles of Management.
- **Electives (9 cr):** Introduction to the Winter Olympics · MKTG 4780 Sports Marketing · Principles of Sports Management · Event Management & Facility Operations · Sports Analytics · Sports Media · Law and Sports.

### 09 — INTEGRATION WITH THE U
- **Layout:** Hub-and-spoke (Business of Sports center, departments orbiting).
- **Spokes:** Law · Parks/Rec/Tourism (Sports Mgmt major partnership) · Humanities (Journalism, Comms, Media) · Engineering (Data Science) · Kinesiology (Sports Medicine) · Business Economics QAMO (Analytics, QAMO 3100) · Marriott Hospitality Initiative · Marketing (Brand Management) · Entrepreneurship (Lassonde, Sport Product Dev) · Information Systems (Student Gameday Competition) · Finance/Accounting.
- **Message:** This minor isn't a silo. It's the connective tissue.

### 10 — UTAH SPORTS ECOSYSTEM
- **Layout:** Eight-column ecosystem grid.
- **Categories:** Major League · Emerging League · Recreation & Resorts · Consumer Brands · Health & Wellness · Olympics & Paralympics · NGBs · Events & Orgs.
- **Anchor logos:** Jazz, Hockey Club, RSL, Royals · Stars, Talons · Park City, Solitude, Snowbird, Brighton, Deer Valley, Powder Mountain, Sundance, Woodward, Eagle Point · Amer Sports, Backcountry, Black Diamond, Cotopaxi, DPS, Kuhl, Petzl, POC, Scott, Skullcandy · Gnarly, LifeVantage, Momentous, MTN OPS, NordicTrack, Nutricost, Zyia · 2034 OPG, USOPC, Paralympics · US Ski & Snowboard, US Speedskating, US Ski Team · Ragnar, Sports Salt Lake, Utah Olympic Legacy.
- **Audience:** Internal + industry. Proves the home court.

### 11 — INDUSTRY PARTNER VALUE
- **Layout:** Two-column — pitch left, pipeline right (already comped, Direction 003 slide 02).
- **Value props:**
  1. Industry perspective on skills, trends, and curriculum focus.
  2. Capstone & internship pipeline — incl. French Alps Olympic Internship, Nice, France.
  3. Connection to Utah's full sports ecosystem (leagues, brands, NGBs, Olympic legacy).
  4. Founding advisory seat — high-impact, focused time commitment.

### 12 — IMPLEMENTATION PLAN & SCHEDULE
- **Layout:** Quarterly timeline grid (Fall 2025 → Q4 2027).
- **Swimlanes:** Program Development · Advisory Group · Curriculum Build · Classroom Launch · Experience Build.
- **Milestones:** Fall '25 student research + advisor kickoff · Q1 '26 draft curriculum · Q2 '26 curriculum framework to academic board · Q3 '26 Intro to Sports Business class launches · Q1 '27 Sports Marketing class · Q3 '27 program officially launches · Olympic engagement + French Alps Internship Program (Nice).

### 13 — ADVISORY GROUP DISCUSSION
- **Layout:** Three-question prompt screen.
- **Questions:**
  1. What are you most excited about regarding our Business of Sports concept? Are there key issues we're missing?
  2. Does the focus — Analytics, Brand, Experience — make sense for the sports industry today and where it's headed? Where would you adjust, add, or refine?
  3. To ensure our students get hired and stand out, what are the most important factors we need to take into account in building the program?

### 14 — WHAT'S NEXT
- **Content:** Where we need your support · Next meeting · Closing remarks · *Shaping This Together.*

### 15 — CLOSING
- **Layout:** Cinematic Rice-Eccles night fireworks (already in source).
- **Headline:** *Ascent Begins Here.* (italic, treated as a signature).
- **Sub:** *David Eccles School of Business | Business of Sports.*

---

## Next steps

1. Internal team reviews the three live comps in `index.html`.
2. Downselect (one direction, or one with a single borrowed element from another).
3. Lock the brand fonts (Iskra + Open Sauce Sans via Adobe Fonts) for the production build.
4. Source final Utah Athletics imagery from UMC, balanced across men's / women's / MUSS.
5. Build out slides 02, 03, 06, 08, 09, 10, 12, 13, 14, 15 in the chosen direction.
6. Wire up interactivity for any data viz (filters on the 2×2 competitive map, partner-logo carousel on the ecosystem slide, timeline scrubber on the implementation plan).

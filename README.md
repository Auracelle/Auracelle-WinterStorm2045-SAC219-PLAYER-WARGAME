# WinterStorm2045 — Live, Fifth Edition DC v2

**Stress-testing NATO's governance capacity across the Arctic grey zone.**

WinterStorm2045 is a quantitative governance wargame built for **NATO STO SAS-219 (SAC-219), High North Scenarios for Wargaming and Analysis**. Players take the Blue Team role and work through Arctic hybrid and grey-zone crises against a Red Team, either the Agentic AI Red Team or a human opponent. The game stress-tests NATO's institutional response round by round: Article 4/5 consultation thresholds, the NATO Capacity Gap, concessions, cognitive and narrative warfare, arbitration and attribution under uncertainty. Every session is scored live against Win-Win, Win-Loss and Standoff outcomes.

Developed independently by **Grace-Alice Evans**, Founder & Principal Investigator, Auracelle AI Governance Labs LLC. The instrument runs on the **E-IAIG-HT framework** (Enhanced Intent–Autonomy–Interaction–Governance — Hierarchical Theory), Fifth Revised Edition, Rev. 1.

> **Build:** Fifth Edition DC v2 · **Framework:** E-IAIG-HT Fifth Revised Edition, Rev. 1 · **Verification:** 13 of 13 framework test vectors pass on load
> **Classification:** Unclassified // For Official Use // SAC-219 Panel Only

---

## Contents

1. [Running the simulation](#running-the-simulation)
2. [Access](#access)
3. [How a session plays](#how-a-session-plays)
4. [What's in the instrument](#whats-in-the-instrument)
5. [Scenarios](#scenarios)
6. [Mathematical foundation and verification](#mathematical-foundation-and-verification)
7. [Adjudication and the White Cell](#adjudication-and-the-white-cell)
8. [The Agentic AI Guide](#the-agentic-ai-guide)
9. [AI features and their limits](#ai-features-and-their-limits)
10. [Environmental Intelligence](#environmental-intelligence)
11. [Data, saving and export](#data-saving-and-export)
12. [External services and dependencies](#external-services-and-dependencies)
13. [Known limitations](#known-limitations)
14. [Repository structure](#repository-structure)
15. [Status, IP and citation](#status-ip-and-citation)

---

## Running the simulation

WinterStorm2045 is a single self-contained HTML file. There is no build step, server or installation.

- **GitHub Pages:** enable Pages for this repository (Settings → Pages → deploy from the `main` branch, root folder). `index.html` is served as the home page, and `.nojekyll` makes Pages serve the file as-is.
- **Locally:** open `index.html` in a current version of Chrome, Edge, Firefox or Safari.

This is the **Live** build. It needs an internet connection for its script libraries and live feeds (see [External services](#external-services-and-dependencies)), so it is **not for offline or air-gapped use**. Each feed falls back to clearly labelled synthetic data when unavailable.

## Access

The simulation opens on a login page. Credentials are issued to SAC-219 panel members separately and are not published in this repository. Two access levels exist:

- **Panel credentials:** full access to the Simulation and the Governance Workbench.
- **Team access code:** a restricted view for the Disruptive Capabilities (R4) workstream.

## How a session plays

The Agentic AI Guide walks players through each step.

1. **Landing page.** The guide summarises the instrument and offers three routes: **Enter Simulation** to play, **Enter Governance Workbench** to conduct a policy, treaty or process assessment, or **Watch the Demo** for a scripted end-to-end playthrough.
2. **Scenario Build.** Choose a scenario, a play mode (Human vs Agentic AI Red Team, or Human vs Human on one device or by asynchronous file handoff), an adversary doctrine and the number of moves. Then start the game.
3. **Crisis Overview.** A briefing sets out the scenario, the actors and the stakes.
4. **Live Theatre.** The scenario plays out on a map with timed decision points and the Article 4/5 Escalation Ladder. Each Blue move ends the turn: resolving a decision point, using the Command Panel, logging a concession, running Cognitive Warfare, or opening the Contested Table.
5. **Red Team response.** The Agentic AI Red Team answers under its doctrine (Russia, Narrative-First; China, Platform-First; or Russia and China, Compound Hybrid), or a human Red Team enters its move. The guide reads each move and its measured effect.
6. **After-Action Report.** When the last move is complete, the report opens with the outcome, a chronological Blue/Red timeline and next steps. From there players can go to **Decision Intelligence** or **Governance Analytics**, **Start Another Game**, or **Log Out of Simulation**.

The header also has **End Game**, which asks for confirmation mid-game and becomes **Start Another Game** once a game ends.

## What's in the instrument

### Simulation

| Tab | Purpose |
|---|---|
| 00 Scenario Build | Choose the scenario, play mode, doctrine and number of moves |
| 01 Live Theatre | Map, decision points, Command Panel, Article 4/5 Escalation Ladder, 3D Terrain View |
| 02 Environments | Arctic operating conditions (EOC) and Environmental Intelligence, and how they shape decisions |
| 03 Overview | Crisis briefing |
| 04 Actor Analysis | Actor governance-capacity profiles and thresholds |
| 05 Concession Engine | Concessions, the Contested Negotiation Table and the Arbitration Track |
| 06 Cognitive Warfare | Narrative and cognitive operations analysis |
| 07 NATO Cap Gap | The NATO Capacity Gap by domain, with manual adjustments |
| 08 Decision Intelligence | What drove the score and where the session turned |
| 09 Players Cognitive Behavior | Decision patterns and cognitive-behaviour scoring |
| WC White Cell | Semi-rigid adjudication: rulings, overrides, sealed scenario causes and the calibration signal |

A **Shared Move Feed** shows every Blue and Red move with its provenance. **Fog of War** can show the NATO Capacity Gap as a band rather than an exact figure.

### Governance Workbench

| Tab | Purpose |
|---|---|
| Narrative Analysis | Assessment of adversary narratives |
| Governance Lab | Scores a policy, treaty or process document (PDF, Word or scanned image) against NATO 1949 and grey-zone governance gaps |
| Governance Analytics | Live E-IAIG-HT figures, the Fifth Edition verification panel, PSTOA, treaty performance, the Evidence Ledger, Monte Carlo projection and the QUBO Optimizer |
| Capacity Cards | Theatre-level capacity cards for GIUK Gap, the Northern Sea Route and Svalbard, in the Disruptive Capabilities (R4) deliverable format |
| OSINT Feed | Open-source news context |

### Live Theatre map

The **Decision-Pressure Field** is the default map. On a polar Arctic projection, it spreads the live Article 4/5 Escalation Composite outward from the incident as a continuous field. Contours mark the framework's zone thresholds (Article 4 at 40, Article 5 at 70, past Article 5 at 90). Propagation routes run to the nearest allied nodes, Red pressure routes grow with Red Team moves, and local refinement tightens while a decision is pending. It shows decision pressure, not a blast radius, and every value comes from the game state. The **Pressure Field** control switches to the classic map with Terrain, Satellite, Infrastructure and Environmental layers. The **3D Terrain View** uses real satellite imagery and elevation data where available.

## Scenarios

There are 17 preset scenarios in three horizon buckets, plus **Build Your Own Scenario** for situations the presets don't cover.

| Bucket | Scenarios |
|---|---|
| **Known** | Svalbard Article 9 Compliance Dispute · GIUK Gap Undersea Cable Interference · Northern Sea Route Access Contestation · Arctic Pipeline Sabotage · Greenland Sovereignty Friction · Bering Strait Grey-Zone Signal Jamming · Barents Sea Energy Coercion · Svalbard Fibre Link EEZ Vessel Loitering · Arctic Icebreaker Gap Exploitation · Compound Hybrid Arctic Pressure Campaign |
| **Unknown — 2030** | Arctic Dual-Use Research Station Biosecurity Incident · Arctic Council Disinformation Cascade · Predictive Failure at Thule/Pituffik · Nordic Airspace GPS/PNT Degradation — Civil-Military Jurisdiction Gap |
| **Unknown — 2045** | Svalbard Satellite Ground Station Interference · Arctic Electromagnetic Spectrum Disruption · Greenland Slope Collapse — Methane Hydrate Event |

**Greenland Slope Collapse** carries a **sealed cause**: natural hydrate destabilisation, the mining operation, or sabotage made to look natural. The White Cell may seal the cause before players see any evidence; otherwise the rules draw it from the scenario's prior probabilities. Survey evidence and the effect of each choice depend on the hidden cause, so attribution decisions are scored against ground truth the players cannot see.

## Mathematical foundation and verification

WinterStorm2045 implements the E-IAIG-HT Fifth Revised Edition, Rev. 1:

- **One canonical governance-capacity equation** (g-GWC), with institutional (G_inst) and environment-adjusted (G_eff) forms and a single combined environmental factor, Φ.
- **Environmental & Weather Operating Conditions (EOC)** for the 2030 and 2045 horizons, with geometric interpolation between them. Known scenarios use 2030 conditions.
- **Environmental Intelligence (EI)** from temperature and non-tidal water level, counted once in the escalation score and applied as drag only to environment-sensitive domains.
- **The Article 4/5 Escalation Composite** on the institutional NATO Capacity Gap, with zones at 40, 70 and 90. Zone labels are game conventions indicating modelled escalation pressure; invoking Article 4 or 5 is a political decision of Allies.

**Verification.** On every page load the build recomputes the framework's Tier 1 test vectors (TV-1 to TV-13) from its own functions, to a tolerance of ±0.005. The login page shows the pass count, and the full table is in **Governance Analytics → Fifth Edition Verification**.

**Uncertainty.** Monte Carlo projection reports outcome probabilities with standard errors and a sensitivity check. The QUBO Optimizer solves the governance-allocation problem by classical simulated annealing; it does not run on quantum hardware.

**Calibration status.** Panel-judgement parameters are analyst-provisional, pending the structured elicitation protocols in the framework (IDEA, swing weighting, the Cooke Classical Model, contrasting groups and modified Angoff, under the NATO SAS-087 Code of Best Practice). WinterStorm2045 is a scenario-conditional wargaming instrument, not a forecasting model.

## Adjudication and the White Cell

WinterStorm2045 uses **semi-rigid adjudication**: the math rules by default, and White Cell judgment steps in only where the rules run out or a result needs overriding, with the reason logged.

- **Contested Table** trades are decided by rule (ACCEPT, EXPLOIT or ESCALATE). Offers too close to call are referred to the White Cell.
- **Arbitration rulings** are decided by rule, so the same case always produces the same result. The language model, where available, only writes the tribunal's wording.
- **Overrides** require a stated reason, and the log keeps both the rule's result and the White Cell's.
- **Draft with AI** proposes a ruling and rationale for the White Cell to accept, edit or reject. Drafts are never applied automatically.
- The **calibration signal** reports override rate and mean shift by source, showing where rule parameters need recalibrating.

## The Agentic AI Guide

A guide panel narrates the session from the landing page to the After-Action Report:

- It welcomes players, explains each route, and walks them through building and starting a scenario.
- It introduces the Live Theatre and reads every Blue and Red move with its measured effect on the NATO Capacity Gap and the Article 4/5 composite. Red moves name the adversary and doctrine.
- It sends players to **Environments** when Arctic conditions change a move's effect, and to the **White Cell** when a ruling is waiting.
- At game end, it reads the result and recommends whether to go to **Decision Intelligence** or **Governance Analytics** first.

**Read aloud** uses the browser's built-in speech. Clicking it reads the current message straight away. The guide narrates from the game's own scores, so it works without any AI service and never describes an effect the model didn't produce. It stays quiet during the scripted Demo, which has its own narration.

## AI features and their limits

The Agentic AI Red Team's move generation, the Blue advisor, narrative analysis, tribunal wording and White Cell drafts call the Anthropic API directly from the browser. Without a proxied key, each falls back to a scenario-aware local engine or template; this is expected behaviour, not a bug. **Scoring and adjudication never depend on the language model**, so outcomes are identical with or without it.

## Environmental Intelligence

The Live build attempts two NOAA feeds:

- **Temperature:** NWS observations at Utqiagvik, AK (station PABR). A 24-hour mean is compared with day-interpolated NOAA 1991–2020 normals.
- **Water level:** NOAA CO-OPS station 9468756, Nome, AK. The 24-hour mean of the non-tidal residual (observed minus predicted tide) is used.

Each variable falls back on its own to the framework's synthetic baseline (+3.5 °C, +10 cm), labelled as such. Live fetches depend on the user's browser and network honouring NOAA's cross-origin settings. These are Arctic-representative US stations, not readings for every scenario location.

## Data, saving and export

- **Autosave:** sessions are saved in the browser's local storage and can be resumed after login. Logging out after a finished game clears the saved session.
- **Session export:** a JSON record (schema 1.1) with the full move log, scores, the institutional and displayed Capacity Gap, the adjudication log and summary, and the build version.
- Nothing is sent to an Auracelle server. The only outbound requests are those listed below.

## External services and dependencies

| Service | Used for |
|---|---|
| `cdnjs.cloudflare.com` | pdf.js 3.11.174 (Governance Lab PDF reading), three.js r128 (3D Terrain View) |
| `cdn.jsdelivr.net` | mammoth 1.6.0 (Word documents), tesseract.js 5 (scanned documents) |
| `api.anthropic.com` | Optional AI features (see above) |
| `api.weather.gov`, `api.tidesandcurrents.noaa.gov` | Environmental Intelligence |
| `server.arcgisonline.com`, `s3.amazonaws.com` | Satellite imagery and elevation tiles for the 3D Terrain View |
| `api.gdeltproject.org` | OSINT Feed |

## Known limitations

- Panel-judgement parameters, including the White Cell rule values and Scenario 12's cause probabilities, are analyst baselines pending structured elicitation.
- Map coastlines in the Decision-Pressure Field are simplified outlines for orientation, not survey-accurate.
- Monte Carlo sampling of BGC scores and EOC coefficients (framework §6.1) is not displayed in this build.
- Read aloud depends on the browser and the system's installed voices. Some embedded viewers don't support speech.
- If players move faster than the voice reads, narration queues and plays in order.

## Repository structure

```
.
├── index.html     The complete simulation (Fifth Edition DC v2)
├── README.md      This file
├── CHANGELOG.md   Build history
├── LICENSE        Copyright and use notice
└── .nojekyll      Serve index.html as-is on GitHub Pages
```

## Status, IP and citation

Active iterative development. Unclassified // For Official Use // SAC-219 Panel Only.

The E-IAIG-HT framework and the Auracelle simulation suite are the intellectual property of Auracelle AI Governance Labs LLC and are the subject of USPTO provisional patent applications. See `LICENSE` for terms of use.

**Suggested citation:** Evans, G.-A. (2026). *WinterStorm2045: Live Governance Wargaming Instrument, Fifth Edition DC v2.* Auracelle AI Governance Labs, for NATO STO SAS-219.

© 2026 Auracelle AI Governance Labs LLC · Evans, Grace-Alice (Ms.) — Founder & Principal Investigator

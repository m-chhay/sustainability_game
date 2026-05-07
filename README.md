# Data Center Sustainability Strategy Optimizer

An interactive planning tool for technology leaders to model the 
financial and environmental impact of data center sustainability 
investments.

Live demo: https://m-chhay.github.io/sustainability_game/

Best experienced on desktop.

---

## What it does

Users configure a data center by dragging sustainability upgrades 
into a slot-based grid. Every configuration produces real-time 
projections across six dimensions:

- **Financial** — total CapEx, annual savings, break-even timeline, 
  5- and 10-year net returns, and annual ROI on capital
- **Environmental** — CO₂ saved (tons/yr), tree-seedling equivalents, 
  PUE and WUE vs. industry benchmarks
- **Deployment** — phased implementation roadmap (0–90 days through 
  2–3 years) with per-phase cost and emissions breakdowns
- **Compliance** — CSRD, Scope 2/3, ISO 50001, RE100, SEC Climate 
  coverage mapped to each upgrade
- **Peer benchmarking** — PUE and WUE compared against Google, 
  Microsoft, AWS, and the Uptime Institute industry average
- **Business case export** — formatted summary with CFO talking 
  points, ready to copy into a presentation

Facility size scales from Edge (~1 MW) to Hyperscale (~100 MW). An 
internal carbon price toggle ($0–$200/ton) and energy rate slider 
show how ROI shifts under different assumptions.

---

## Data sources

Financial estimates are calibrated to a 5 MW mid-size baseline and 
derived from peer-reviewed studies, government reports, and vendor 
case studies:

- EPA GHG Equivalencies Calculator (tree, car, flight conversions)
- IEA World Energy Outlook 2024
- Lawrence Berkeley National Laboratory (solar savings)
- Cornell University (2025) — AI data center emissions roadmap
- Google Environmental Report 2023; Microsoft Sustainability Report 2023
- California Energy Commission (2024); Applied Energy / ScienceDirect
- Uptime Institute Global Data Center Survey 2023 (PUE/WUE baselines)

Figures are illustrative and intended for planning conversations, 
not formal capital projections.

---

## Why I built this

Most sustainability ROI tools are either locked inside enterprise 
software or too abstract to use in a real stakeholder conversation. 
I wanted something a technology leader could open in a browser, 
configure in five minutes, and walk into a board meeting with.

The project combines my interest in sustainability strategy, 
enterprise infrastructure, and data-driven decision-making.

---

## Tech stack

Single-file HTML/CSS/JS — no build system, no dependencies, 
works offline. Drag-and-drop built with native HTML5 Drag API. 
Charts and benchmarks rendered with vanilla DOM/SVG.

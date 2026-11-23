# Research Tracker (English version) v1.3

A single-file web app developed independently for overseas / English-speaking users, derived from "科研工作台（多语言）v1.0.2".

## Core differences from the Chinese multilingual version

| Dimension | Chinese multilingual (zh) | English (this version) |
|---|---|---|
| UI language | Simplified Chinese + Traditional Chinese (Hong Kong) | English only (no switcher; no Chinese text in the UI) |
| Journal auto-match | Keeps easyScholar open API (fill your own key) | Removed (depends on a domestic service, unusable overseas) |
| Journal tier system | JCR / CSSCI / CSCD / CCF / Peking Core / EI / Scopus … | International tiers only (see below) |
| Settings dialog | API key + your name | Your name only (no key) |
| New project form | Chinese / English / Bilingual + Chinese examples | English only + English examples |

## Journal tiers (international system)

- **JCR Q1 – Q4**
- **Scopus** (no quartile; marked when matched)
- **EI** (Engineering Index)
- **English General Journal** (manual mark when not indexed above)

v1.1 changes: removed CAS, SCI/SSCI/AHCI/ESCI; Scopus merged from Q1–Q4 into a single Scopus. The card badge shows the highest-priority tier.
v1.2 changes: discipline classification fully in English (JCR / Web of Science codes, e.g. SOCIOLOGY / URBAN STUDIES); internal storage changed from Chinese names to English codes.
v1.3 changes (2026-11-23): ported the offline-capable features from cloud v2.2.0–v2.2.4 — paper-level "Revising" status (major/minor) with filter & grouping, card stage-duration tag (current stage + elapsed days + current journal & tier), new sort options (by latest stage / by stage duration, ranked Revising > Under Review > Accepted > Rejected > others), and a "Revising" count in the overview row. Also fixed missing UI strings (btnBack / statRejected).

Tiers appear as multi-select chips in the submission form; the card badge shows the highest-priority tier.

## Features kept

Paper folder + multiple submissions model, English titles, author order & co-first/corresponding markers, submission rounds & status tracking, progress timeline, charts (status distribution / tier distribution / top accepted tiers / top-5 submitted journals), CSV / JSON import & export, local storage (data stays on your device).

## Usage

Open `index.html` directly in a browser. No internet, no server required.

## Source

- `index.html` — the application
- (Source-code markdown copies are not included in this repository; the HTML file is the source of truth.)

## Back

[Root README](../README.md) · Chinese version at [`../zh/`](../zh/)

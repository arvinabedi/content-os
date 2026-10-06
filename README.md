# Content OS

**A content-quality dashboard for a multilingual, multi-brand product catalog.** It answers the questions the content team actually asks: which products are missing what, which languages are behind, which categories drag the score down, and how things moved week over week.

| | |
|---|---|
| **Role** | Builder: data model, scoring, UI, deployment and Tool Hub sign-in |
| **When** | September – October 2026 |
| **Stack** | Python (Flask API), React 19 + Vite + TypeScript, SQLite, nginx |
| **Size** | ~18,500 lines with a pytest suite · 13 commits |
| **Status** | Deployed on the company server, signed in through [Tool Hub](https://github.com/arvinabedi/tool-hub) |

> The source is private company code at Ronix Tools. I'm glad to walk through it in an interview. → [Portfolio](https://arvinabedi.github.io)

## Two sources in

1. **The weekly XLSX content report**, parsed and kept as history so any two weeks can be compared
2. **The product CMS's API**, mirrored locally on a schedule, with credentials and sync runs managed from the admin screens

## Eleven sections

| Group | Section | Answers |
|---|---|---|
| Overview | Executive | Headline KPIs for the selected report and brand |
| Overview | Compare | Two reports side by side: what moved |
| Operations | Content | Per-field completeness across the catalog |
| Operations | Gaps | The specific products missing a given field, exportable as a work list |
| Operations | Languages | What exists in one language but not another |
| Intelligence | Forecast | Velocity and estimated completion date per content field |
| Intelligence | Categories | Category-level breakdown and hierarchy |
| Intelligence | Readiness | One composite score per product |
| Intelligence | Report | The raw parsed report, filterable and exportable |
| Admin | Users | Users, roles and per-permission grants |
| Admin | CMS | API connection, sync runs, mirrored products |

## The readiness score

Each product gets one number that a content manager can sort by: **content 70, category 15, SEO 15.** Content is weighted heaviest because a product with a perfect category but no description still can't be sold online.

---

[Portfolio](https://arvinabedi.github.io) · [All case studies](https://github.com/arvinabedi)

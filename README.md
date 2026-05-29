# Corridor Atlas — Baltimore → Richmond Physician Relocation Map

An interactive, single-file map for evaluating where to live and work along the
I-95 corridor between Baltimore, MD and Richmond, VA. Built for a physician
relocation search across two specialty tracks (hospitalist and neonatology).

**Live:** `https://sunnypately.github.io/corridor-atlas/`

## What it shows

- **Hospitals (29)** across MD / DC / VA. NICU/neonatology sites are flagged
  with their level of care; every pin links to that system's careers page.
- **Toll Brothers communities (12)** with starting prices, square footage, and
  build status. Each home auto-computes distance to the nearest hospital and the
  nearest NICU, plus an estimated Walk Score and area school rating.
- **Top public schools (15)** with district and GreatSchools links.

## Controls

- Toggle the hospital / home / school layers independently
- Filter by state (MD / DC / VA)
- Show NICU-only hospitals
- Drag the price-ceiling slider to hide homes above budget
- Average compensation bands for both specialties + direct apply links
  (SHM, AAP PedJobs, PracticeLink, NEJM, Indeed)

## Data notes

- **Researched (May 2026):** Toll Brothers communities, prices, square footage,
  and salary bands — sourced from tollbrothers.com, Salary.com, Indeed,
  ZipRecruiter, and ERI.
- **Estimated:** Walk Scores and school ratings on home pins are approximations
  to orient the search; verify each via the in-app links.
- **Live, not frozen:** Job openings change daily, so the map links to careers
  pages and boards rather than listing static postings.
- Toll Brothers builds little in metro Richmond — the home layer concentrates in
  Northern Virginia and the Maryland DC suburbs.

## Stack

Self-contained `index.html`. Leaflet + CARTO dark tiles, no build pipeline.

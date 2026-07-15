# Klaus Miller Academic Website

## Overview
Static HTML/CSS academic website for Klaus Miller, Assistant Professor of Quantitative Marketing at HEC Paris. Hosted on GitHub Pages at `klausmiller.github.io`.

## Repository
- GitHub: https://github.com/klausmiller/klausmiller.github.io
- Branch: `master`
- Domain: `klausmiller.com` (currently using 1&1 HTTP redirect to `https://klausmiller.github.io`)

## Site Structure
- `index.html` - Landing page with bio, links to Google Scholar, ResearchGate, SSRN, GitHub, LinkedIn
- `research.html` - Working papers, published papers, large-scale collaborative research, conference proceedings, book
- `talks.html` - Invited talks and conference presentations. Two sections: "Selected Invited & Industry Talks" (linked/recorded — INMA, Oxera, PMDS videos) and "Conference Presentations and Invited Seminars" (year-grouped, old-Google-Sites style, `*` = co-author presented). Seeded from CV (`Conference Presentations and Invited Seminars` section); 2024-2026 use the old website's curated wording verbatim, 2023 and earlier seeded from CV
- `awards.html` - Research and teaching awards
- `teaching.html` - HEC Paris teaching experience (Grande Ecole, MBA/EMBA, PhD, Summer School)
- `media.html` - Media appearances and press coverage (clickable titles, paper references). Invited/industry/recorded talks were split out to `talks.html` (June 2026)
- `contact.html` - Contact information
- `style.css` - Stylesheet with classes: `.venue` (italic journals), `.highlight` (bold awards), `.year`, `.plain` (no bullets), `.name`, `.container` (760px max)

## Files Not in Navigation
- `education.html` - Removed from git (excluded from navigation)
- `images/` - Profile image removed from landing page, folder cleaned from git

## Domain Setup
- Domain registrar: 1&1 (1und1.de / IONOS)
- Current setup: HTTP redirect from `klausmiller.com` to `https://klausmiller.github.io`
- The redirect target MUST include `https://` prefix or it causes an infinite redirect loop
- Ideal setup: Set A records at 1&1 pointing to GitHub IPs (185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153) and add CNAME file to repo. This requires finding DNS settings at 1&1 (under Domains & SSL > DNS, not under redirect settings).

## CSS Classes Reference
- `.venue` - Journal names (italic)
- `.highlight` - Awards and distinctions (bold)
- `.year` - Year labels
- `.plain` - List without bullets
- `.name` - Nav name link
- `.active` - Current page nav highlight
- `.container` - Main wrapper (max-width 760px)
- `.profile-img` - Profile image (currently unused)

## Content Sources
- CV file: `C:\Users\millerk\HEC PARIS Dropbox\Klaus Miller\000_Admin\HEC\09_AcademicActivityReporting\05_2025-2026\miller_cv-2026-01-29.docx`
- Previous website: https://sites.google.com/view/klausmiller (Google Sites, being replaced)

## Key Decisions
- "Sophisticated Consumers with Inertia" listed as "Conditionally Accepted" at AER on the public website (updated 2026-07-14; still under Working Papers until fully accepted)
- "The Sources of Researcher Variation in Economics" (Many Economists Collaborative) listed as "Conditionally Accepted" at Journal of Economic Literature on the public website (updated 2026-07-15; was "Revise and Resubmit")
- Media page: Titles are clickable links (where URL exists), no separate [Link]/[Video] lines
- Media entries reference the underlying paper with "On: Paper Title" linking to SSRN/journal
- Teaching page shows HEC Paris experience only (no Goethe University)
- Copyright footer: 2026 on all pages
- No profile image on landing page
- Education page excluded from navigation

## Change Log

### February 2026 - Initial Migration
- Migrated website from Google Sites to static HTML/CSS
- Set up GitHub Pages hosting at klausmiller.github.io
- Removed profile image from landing page
- Excluded education from navigation
- Standardized nav across all pages: Home | Research | Awards | Teaching | Media | Contact

### February 2026 - Content Updates
- Updated landing page bio text (multiple revisions, final version is concise 4-paragraph bio)
- Made paper titles clickable on research page (links to SSRN/journal)
- Removed author affiliations from research page
- Expanded media page with all mentions from Google Sites research page
- Added paper references ("On:") to media entries
- Added Engagement vs. Commitment paper (SSRN 5520458) to research and media
- Added CNIL events (GDPR Economic Impact with Aghion, Privacy Research Day 2024)
- Added YouTube videos (HEC Data in Advertising, Privacy Violations talk)
- Updated copyright to 2026 on all pages
- Removed unused files from git (education.html, images/)

### February 2026 - CV-Based Updates
- Updated teaching page with HEC Paris experience from CV (replaced Goethe University content)
- Added 9 missing media mentions from CV since 2015:
  - Knowledge@HEC on GDPR on Online Tracking (2025)
  - Datagrail, Ad Exchanger, Cornerstone Research on Privacy Violations (2024)
  - Law.com on Paying for Privacy (2024)
  - Meta and Data Privacy, Knowledge@HEC (February 2022)
  - S&P Global Market Intelligence (April 2018)
  - Into the Minds Blog (2017)
  - Planung & Analyse Online (2017)

### February 2026 - Media Page Redesign
- Made media headlines clickable (link wrapped in title instead of separate [Link]/[Video] line)
- Shortened page by removing redundant link lines

### June 2026 - Added Talks Page
- Created `talks.html` to separate invited research/industry talks and conferences from media coverage
- Added "Talks" to nav across all 7 pages (Home | Research | Talks | Awards | Teaching | Media | Contact)
- Moved 4 entries from `media.html` to `talks.html` ("Selected Invited & Industry Talks"): INMA Master Class (2026), Oxera roundtable (2026), two recorded Platforms/Markets/Digital Society talks (2025, 2024)
- "Conference Presentations and Invited Seminars": comprehensive year-grouped 2017-2026 seeded from CV `miller_cv-2026-05-07d.docx`, deduped per year, sorted newest-to-oldest within year, `*` = co-author presented. Includes planned 2026 talks per KM. CV has no 2015-2016 conference entries, so the list begins 2017 (KM's "since 2015 at Goethe" rule). Pre-2017 WTP/dissertation-era talks (2006-2014) intentionally excluded
- KM decisions applied: YES Basel + Weizenbaum kept under 2024; a second (Oct 2025) Weizenbaum added under 2025; old-site-only 2025 seminars retained (Columbia, Maryland, Kansas, Kelley, NYU Law, CUHK, UK Digital Economics Workshop); borderline items (CNIL/Aghion, HEC "Data in Advertising" video, CGTN) left in `media.html`
- Open polish: two old-site hyperlinks (European Quant Marketing Workshop, INRIA BALANCE Workshop) not yet re-added (URLs pending from KM); a few `*` attributions on older years worth a spot-check
- Committed and pushed to master

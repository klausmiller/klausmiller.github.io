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
- `media.html` - Media appearances and press coverage (clickable titles, paper references). Invited/industry/recorded talks were split out to `talks.html` (June 2026). Three sections: "Policy & Regulatory Citations" (regulators/legislatures citing his papers directly), "Cited in Litigation" (court filings), "Press Coverage" (everything else, added July 2026)
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

### July 2026 - Policy & Regulatory Citations Section
- Added "Policy & Regulatory Citations" and "Cited in Litigation" subsections to `media.html`, above "Press Coverage" (which was previously an unheaded flat list)
- Every entry was independently verified by downloading the primary source (regulator PDF/HTML) and confirming the exact citation text, page/footnote, and that it refers to this Klaus Miller (not another researcher of the same surname) before publishing
- Policy & Regulatory Citations (reverse-chronological): AGCM Italy Apple ATT decision (Dec 2025, replaces the old thinner AGCM media.html entry — the decision itself cites the 18-23% publisher-revenue estimate from "Economic Value of User Tracking", Section 72 n.79); FTC Negative Option Rule (Oct 2024, cites "Sophisticated Consumers with Inertia", nn.538-539); OECD Competition Committee note by Poland (June 2024, n.7); UK ICO "consent or pay" consultation, third-party academic submission (Apr 2024, cites "Pay-or-Tracking Walls", n.7); CNIL-commissioned economic study by Telecom Paris (Feb 2024, cites three papers)
- Cited in Litigation (separate subsection per KM's explicit choice, not folded into regulatory citations): Zeithammer expert report in *In re Google RTB Consumer Privacy Litigation* (N.D. Cal., 2023)
- KM decision: dropped two FTC-hosted PrivacyCon/workshop research papers (by other authors, hosted on ftc.gov but not the FTC's own regulatory text) that a broader search also surfaced — KM wanted the regulatory section limited to the regulator's/legislature's own citing text, not third-party papers merely hosted on a .gov domain
- Note for KM: the ICO citation of "Pay-or-Tracking Walls" gives co-author as Timo Muller-Tribbensee (SSRN abstract_id=4749217, posted March 2024), not Rene Laub as currently listed as the PUR collaborator in project memory/research.html (which shows the paper as an unlinked working-in-progress) — worth reconciling authorship/link on `research.html` next time that project is touched; not changed here since it's outside a media-page task
- Search process: ran a 19-agent Workflow sweep across all research.html papers x 11 regulatory ecosystems (FTC, EU Commission, UK CMA/ICO, CNIL, AGCM/Garante, Bundeskartellamt/BfDI, EDPB/EDPS, US Congress/GAO, OECD/EU Parliament, state AGs/court filings, other national DPAs). Caught and hand-corrected a scratch-file race condition in the workflow's verify stage (concurrent agents sharing a generic filename like `verify.pdf`, silently overwriting each other's downloads mid-fetch) that had produced a false rejection of the AGCM citation and other unreliable verdicts; every surfaced candidate was re-fetched and re-checked manually with unique filenames before being trusted

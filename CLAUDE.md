# Klaus Miller Academic Website

## Overview
Static HTML/CSS academic website for Klaus Miller, Assistant Professor of Quantitative Marketing at HEC Paris. Hosted on GitHub Pages at `klausmiller.github.io`.

## Repository
- GitHub: https://github.com/klausmiller/klausmiller.github.io
- Branch: `master`
- Domain: `klausmiller.com` (currently using 1&1 HTTP redirect to `https://klausmiller.github.io`)

## Site Structure
- `index.html` - Landing page with bio, links to Google Scholar, ResearchGate, SSRN, GitHub, LinkedIn
- `research.html` - Published & accepted papers, working papers, industry publications (HBR), conference proceedings, book
- `talks.html` - Invited talks and conference presentations. Two sections: "Selected Invited & Industry Talks" (linked/recorded — INMA, Oxera, PMDS videos) and "Conference Presentations and Invited Seminars" (year-grouped, old-Google-Sites style, `*` = co-author presented). Seeded from CV (`Conference Presentations and Invited Seminars` section); 2024-2026 use the old website's curated wording verbatim, 2023 and earlier seeded from CV
- `awards.html` - Titled "Awards & Service". Three sections: Research Grants, Editorial & Reviewing, Fellowships & Invitations. Nav label is still the single word "Awards"
- `teaching.html` - HEC Paris teaching experience (Grande Ecole, MBA/EMBA, PhD, Summer School)
- `media.html` - **Titled "Impact"** (nav label, `<h1>` and `<title>`); the **filename stays `media.html`** so existing links from the CV, papers and bookmarks keep working. Regulatory citations, litigation and press coverage (clickable titles, paper references). Invited/industry/recorded talks were split out to `talks.html` (June 2026). Three sections: "Policy & Regulatory Citations" (regulators/legislatures citing his papers directly), "Cited in Litigation" (court filings), "Press Coverage" (everything else, added July 2026)
- `contact.html` - Contact information
- `style.css` - Stylesheet with classes: `.venue` (italic journals), `.highlight` (bold awards), `.year`, `.plain` (no bullets), `.name`, `.bio` / `.bio-text` / `.bio-photo` (two-column bio), `.container` (920px max)

## Files Not in Navigation
- `education.html` - Removed from git (excluded from navigation)
- `images/` - Removed from git; the portrait lives at the repo root as `profile.jpg`

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
- `.container` - Main wrapper (max-width 920px)
- `.bio` - Two-column bio wrapper (flex)
- `.bio-text` - Left text column
- `.bio-photo` - Right portrait column (270px)

## Content Sources
- CV file: `C:\Users\millerk\HEC PARIS Dropbox\Klaus Miller\000_Admin\HEC\09_AcademicActivityReporting\05_2025-2026\miller_cv-2026-01-29.docx`
- Previous website: https://sites.google.com/view/klausmiller (Google Sites, being replaced)

## Key Decisions
- "Sophisticated Consumers with Inertia" listed as "Forthcoming, American Economic Review" under Published & Accepted Papers (accepted 2026-09; was "Conditionally Accepted" under Working Papers from 2026-07-14)
- "The Sources of Researcher Variation in Economics" (Many Economists Collaborative) listed as "Accepted, Journal of Economic Literature" under Published & Accepted Papers (updated 2026-08-17; was "Conditionally Accepted" under the now-dissolved collaborative section)
- No separate "Large-Scale Collaborative Research" section — consortium papers sit in the regular lists with a one-line "with [leads], and the [Collaborative]" attribution (KM decision, 2026-08-17)
- Harvard Business Review pieces live in their own "Industry Publications" section, not mixed into Published & Accepted Papers (KM decision, 2026-08-17)
- Media page: Titles are clickable links (where URL exists), no separate [Link]/[Video] lines
- Media entries reference the underlying paper with "On: Paper Title" linking to SSRN/journal
- Teaching page shows HEC Paris experience only (no Goethe University)
- Copyright footer: 2026 on all pages
- Profile photo: `profile.jpg` is the **full-length** official HEC portrait 2026, uncropped 3:4, 810x1080 px. The bio is a two-column flex (`.bio`): text column left (`.bio-text`), portrait column right (`.bio-photo`, 270px). Below 600px it stacks `column-reverse`, photo above the text at 175px. No photo in the nav, and the text no longer wraps around the photo (KM, 2026-10-15)
- **No title line in the header.** One was added on 2026-10-06 and removed on 2026-10-07: KM found it made the header heavy. The header is name + nav only. Position is still "Assistant Professor of Marketing" everywhere it appears, incl. the `index.html` `<title>`
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
- Follow-up sweep (same day) targeting Apple ATT cases specifically (Bundeskartellamt, Autorite de la concurrence, UOKiK, EU Commission DMA, UK CMA, US DOJ, ACM, CNMC, others) found nothing new beyond what was already published; Poland's UOKiK has only a preliminary (non-public-decision) ATT investigation open as of June 2024, per the OECD note already cited above
- The search-and-verify pattern was generalized into a reusable Workflow script, `~/.claude/workflows/policy-citation-search.js` (usage guide: `policy-citation-search.md` next to it; pointer memory: [[reference_policy_citation_search_workflow]]) for future sporadic re-checks. A subsequent smoke-test run of that script (meant to be minimal) accidentally ran the full default sweep due to an `args`-passed-as-JSON-string mistake — see [[learn_workflow_args_json_not_string]] — but the resulting run surfaced two more real, independently-verified citations, added same day: European Commission Case DMA.100055 (Meta, Article 5(2) non-compliance, 23 Apr 2025) relying on "Paying for Privacy: Pay-or-Tracking Walls" (recital 93, n.81) — added to Policy & Regulatory Citations; and confirmation that KM personally presented "Perceived Privacy Violations" at FTC PrivacyCon 2024 (6 March 2024), added as a proper linked entry to `talks.html`'s Selected Invited & Industry Talks (was previously just a bare name in the 2024 conference list)

### July 2026 - Policy & Regulatory Citations Simplified
- KM felt the 3-line entries (title/date, citing body, "Cites X paper... — page/footnote") were too long. Dropped the third line (paper-relationship detail) from all Policy & Regulatory Citations and Cited in Litigation entries; now just title+date and citing body/venue, two lines each, matching the rest of the site's minimal style. The specific paper/page citation detail still lives in `~/.claude/workflows/policy-citation-search.md`'s known-citations list if it's ever needed again

### August 2026 - Research Page Restructure (JEL accepted, HBR split out)
- "The Sources of Researcher Variation in Economics" is now **Accepted at the Journal of Economic Literature** (was Conditionally Accepted since 2026-07-15). KM chose the wording "Accepted" over "Forthcoming"
- Dissolved the "Large-Scale Collaborative Research" section per KM. Its two papers moved into the regular lists: the JEL paper to the top of Published & Accepted Papers, the IJRM Reproducibility Collaboration many-analyst preprint to Working Papers (KM's call — it has no journal status yet, so it belongs with the unpublished work)
- Consortium attribution condensed from three lines (collaborative name / lead collaborators with affiliations / status) to the site's standard one-line format: "with Nick Huntington-Klein, Claus Pörtner, and the Many Economists Collaborative (146 research teams)". Same treatment applied to the many-analyst preprint ("with Koen Pauwels, Karin Teichmann, Oliver Koll, Hannes Datta, Harald van Heerde, and the IJRM Reproducibility Collaboration"), dropping the university affiliations that no other entry on the page carries
- New "Industry Publications" section between Published & Accepted Papers and Conference Proceedings, holding both HBR pieces (auto-renew with Z. John Zhang, May 2026; Cookies Are Worth More Than You Think with Bernd Skiera, Nov–Dec 2024). Peer-reviewed and practitioner work are now visibly separated
- Section order on `research.html`: Working Papers → Published & Accepted Papers → Industry Publications → Conference Proceedings → Book
- `index.html` bio: added the *Journal of Economic Literature* to the journal list, named first (KM's request). Sentence changed from "has been published in journals such as" to "is published or forthcoming in journals such as" — the JEL paper is accepted but not yet in print, so the plain "published" claim would have been premature. Also fixed the stray two-item serial comma that the old sentence carried

### September 2026 - JEL article link, SAMS Lausanne talk
- The JEL paper now has an AEA article page (`10.1257/jel.20261837`). Title link on `research.html` repointed from SSRN to the AEA page, matching how every other entry in Published & Accepted Papers links to its publisher; the SSRN preprint kept as a fourth line on the entry so the full text stays reachable while AEA has no published version up
- Status wording changed from "Accepted" to "Forthcoming, *Journal of Economic Literature*" (KM's call, 2026-09-11) - this reverses the August decision, and now matches how AEA itself lists it: forthcoming, no volume/issue/pages assigned yet. `index.html` needed no change (it already reads "published or forthcoming")
- The AEA URL was stored without the `&&from=f` tracking suffix that AEA's forthcoming-articles listing appends
- `talks.html`: added "Swiss Academy of Marketing Science (SAMS) Conference Lausanne (Switzerland)" at the front of the 2026 line (4 September 2026, UNIL). KM presented the polarization paper himself, so no `*`. Placed first because it is the most recent 2026 item
- CV updated in parallel (`miller_cv-2026-09-11a.docx`): same Forthcoming wording plus an AEA link, SAMS added to the "Engagement vs. Commitment" presentation block

### September 2026 - AER, opening paragraph
- `index.html` journal list now leads with the *American Economic Review*, ahead of JEL (commit `08eae07`, together with the AER acceptance on `research.html`)
- `index.html` opening paragraph rewritten per KM (2026-09-30): adds "since 2021" to the Hi!PARIS chair and a new sentence on the career path ("Before returning to academia at Goethe University Frankfurt in 2015, I spent nearly five years in industry"); research focus now reads "with a focus on online advertising, privacy, and the digital economy". HEC Paris and Hi!PARIS links kept; Goethe left unlinked (KM confirmed: no link)
- Hi! PARIS now carries its official name, taken from hi-paris.fr: "Hi! PARIS Center on Data Analytics and Artificial Intelligence for Science, Business and Society" (was "Hi!PARIS Center on Data Analytics and AI"). Uses the institute's own spelling with a space. Homepage only: the grant title (`awards.html`) and talk venues (`talks.html`, `teaching.html`) still read "Hi!PARIS"
- ERC Advanced Grant role and dates corrected (KM, 2026-09-30). Klaus was not officially listed as Co-PI, so his role is now "investigator" everywhere, never "co-investigator" or "Co-PI". Dates are 2019-2026 because the grant was extended. Changed on `index.html` ("an investigator") and on `awards.html`, where the entry was stale at "2019-2024" and "Co-Investigator"
- Homepage bio split from 4 into 7 paragraphs for readability (KM's request). Wording and sentence order unchanged. Breaks: position + career path / research focus + methods / visiting + journals / industry collaboration + media / awards + ERC (unchanged) / editorial + reviewing / conference co-organizing

### October 2026 - New Portrait Photo
- Replaced `profile.jpg` (nav photo on `index.html`) with the official HEC Paris portrait (2026, blue background)
- Cropped to head-and-shoulders at 3:2 so it fits the existing `.nav-photo` slot without CSS changes; downscaled to 600x400 px / ~21 KB (previous file was 5760x3840 px / 4.7 MB)

### October 2026 - Home Page: Portrait Beside the Bio, Title Line, Bio Wording
- Photo moved out of the nav: `profile.jpg` is now a 4:5 head-to-chest crop of the official HEC portrait (600x750 px) floated right of the opening paragraphs via the previously unused `.profile-img-right` (200px; 140px on mobile). The 140px nav thumbnail made the face only ~45px tall; `.nav-photo` CSS removed as unused
- Title line added under the name on all 7 pages: "Assistant Professor of Marketing, HEC Paris - Chairholder, Hi! PARIS Center" (`nav .tagline`). Chosen over a circular-avatar header and a two-column hero (nav loses the name, tagline wrapped badly); mockups of all three were reviewed by KM
- `index.html` `<title>` now "Klaus Miller - Assistant Professor of Marketing" (was "... of Quantitative Marketing", which contradicted the body). KM picked "Marketing"
- Bio reworded, still seven paragraphs at KM's request; all facts, links and venue spans unchanged. Paragraph openings varied (previously all seven began with "I"); journals now lead paragraph 3 ahead of the visiting positions; ERC role stays "investigator", 2019-2026
- Open, suggested 2026-10-05 and not yet decided: a 3-item "Recent" block above the bio, CV (PDF) and ORCID in the Links row, compressing seven paragraphs to four or five

### October 2026 - Homepage Bio Shortened to Four Paragraphs
- Bio cut from 7 paragraphs / 291 words to 4 / 270. Layout deliberately unchanged at KM's request ("layout we can largely leave the same"): same nav, title line, floated portrait, Links section. The "Recent" block and the icon links row that were mocked up were **not** adopted
- Merges: journals + press + visiting positions + awards + ERC into one credentials paragraph; conferences + editorial roles into one service paragraph. The two conference descriptions ("an annual event on...", "a workshop bringing together...") were dropped as the only real content cut; the links carry that information
- **New research statement (paragraph 2).** Replaces "My research sits at the intersection of quantitative marketing, economics, and information systems", which named fields rather than questions. Now two strands: what personal data is worth and who captures it, and why consumers stay in contracts they would not choose again. Deliberately two-stranded so the forthcoming AER paper (auto-renewal / consumer inertia) sits inside the description - a privacy-only framing would have excluded it. KM did not pick between the two drafts offered; the sharper privacy-only alternative can be swapped in as a single paragraph
- No link or journal name dropped: the edit script asserts the `href` set and the `<span class="venue">` set are identical to the previous version, and that the new text is strictly shorter
- Still open: a 3-item "Recent" block, CV (PDF) + ORCID in the Links row, icon links row
- **Inconsistency flagged to KM, not changed:** `index.html` says "IJRM Best Paper Award", `research.html` says "IJRM Best Article Award 2024"

### October 2026 - Research Paragraph Reverted to KM's Own Wording
- Paragraph 2 is **back to Klaus's categorisation**: "My research sits at the intersection of quantitative marketing, economics, and information systems. I study online advertising, privacy, and the digital economy, drawing on econometric methods, causal machine learning, and large-scale field experiments." Verbatim from `9eded1e`
- The two-strand statement Claude had drafted ("what personal data is worth and who captures that value" / "why consumers stay in contracts they would not choose again") is **removed**. It was Claude's wording, not Klaus's. KM will revisit it when his tenure package is available
- The industry-partner sentence from the old paragraph 4 stays appended here, since the four-paragraph merge had folded it into paragraph 2
- Four-paragraph structure and layout unchanged. Bio is now 248 words
- **Standing note:** do not re-propose a rewritten research statement unprompted. KM owns that wording

### October 2026 - Header Title Line Removed
- The title line added under the name on all 7 pages on 2026-10-06 is gone. KM: "it makes it a little bit heavy". Header is back to name + nav
- `nav .tagline` removed from `style.css` (desktop and mobile rules), and `nav .name` margin restored from 2px to its original 10px, since the gap above the nav list was being provided by the tagline
- Net effect: the header is identical to its pre-2026-10-06 state. The position is no longer stated above the fold on the inner pages; on `index.html` the first bio sentence carries it

### October 2026 - Research Page: Published Papers First
- `research.html` section order is now Published & Accepted Papers -> Working Papers -> Industry Publications -> Conference Proceedings -> Book (KM, 2026-10-13). Previously Working Papers led the page
- Pure block swap: no entry, link or wording changed (script asserted identical `<li>` count, `href` set and byte length)

### October 2026 - Home Page: Two-Column Bio with the Full-Length Portrait
- KM asked for "the full body picture on the home page on the right and the text on the left". `profile.jpg` is now the **uncropped** portrait (3:4, 810x1080 px), not the 4:5 head-to-chest crop
- The bio became a real two-column flex rather than a float: `.bio` wraps `.bio-text` (left, flexible) and `.bio-photo` (right, 270px fixed). Text no longer wraps underneath the photo
- Mobile (<=600px): `flex-direction: column-reverse` puts the portrait above full-width text at 175px
- `.profile-img` and `.profile-img-right` removed from `style.css`; both were now unused
- **Trade-off flagged to KM:** at the 270px column the full frame renders his face about 85px tall, against about 108px for the 4:5 crop it replaced. He chose the full picture knowing this. The crop is recoverable from `bd2d94f:profile.jpg`
- Container was 760px at this point; widened to 860px on 2026-10-15, see below

### October 2026 - Wider Container, KM's Methods Wording
- `.container` max-width 760px -> **860px**, site-wide (KM: "make the page a little bit wider"). The home text column is now ~554px beside the 270px portrait; the other six pages simply get wider lines, which suits them because they are mostly short list entries rather than prose
- Methods clause in paragraph 2 replaced with **Klaus's own wording**: "drawing on large-scale field experiments and quasi-experimental methods for causal inference" (was "econometric methods, causal machine learning, and large-scale field experiments"). His words, proposed verbatim in his message
- **Flagged to KM, not decided:** his wording drops "causal machine learning", which his own profile lists among his methods. One clause to add back if that was unintended
- He also floated dropping the methods clause entirely. Kept it, on the argument that methods are a standard and useful signal on an academic homepage, and said so; one edit away if he disagrees
- Bio stays 248 words, four paragraphs

### October 2026 - Container Widened Again to 920px
- KM: "a little bit broader but not much". `.container` 860px -> **920px**, site-wide. Home text column is now ~614px beside the unchanged 270px portrait
- Width progression this day: 760 -> 860 -> 920. Photo column deliberately left at 270px; he asked for width, not a bigger photo
- Committed by partial-staging again, since another session's uncommitted `.paper-links` block still shares `style.css`

### October 2026 - Editorial & Reviewing Moved Off the Front Page
- KM asked to drop "I serve as Guest Associate Editor ... and as an ad-hoc reviewer for ..." from `index.html` and put it "to service somewhere suitable". Paragraph 4 is now just the two Paris conferences; the bio is 4 paragraphs / ~219 words
- The roles moved to `awards.html` as a new **"Editorial & Reviewing"** section, placed between Research Grants and Fellowships & Invitations so current service sits above the historical scholarships. Guest AE (IJRM) and ad-hoc reviewer (ManSci, MktSci, JMR, ISR) as two `ul.plain` entries, matching the page's existing markup
- `awards.html` `<h1>` changed "Awards" -> **"Awards & Service"**, since the page already held grants and fellowships and now holds service too. The **nav label stays "Awards"** to avoid touching all 7 pages; say the word to align it
- There is still **no separate Service page and no 8th nav item**; a 2026-04-27 plan to build a Service section on the front page was never approved and is now moot, since KM wants this off the front page entirely

### October 2026 - Credentials Paragraph Split
- KM asked for a break before "I have been a visiting scholar at the Wharton School...". Journals + press coverage now close one paragraph; visiting positions + ISMS + IJRM award + ERC open the next. Bio is **5 paragraphs / 211 words**
- Pure split: prose, `href` set and `<span class="venue">` set asserted byte-identical to the previous version. No rewording
- Also normalised the bio `<p>`/`</p>` tags to one indentation level. One had been left at the wrong depth by the 2026-10-15 two-column refactor; cosmetic only
- Bio paragraph count over this period: 4 -> 7 (2026-09-30) -> 4 (2026-10-07) -> 5 (now)

### October 2026 - AI@HEC Workshop Added to Talks
- Added "AI@HEC Research Workshop (HEC Paris)" to the **front** of the 2026 line on `talks.html` (internal AI@HEC research workshop, Wed 14 October 2026, convened by Christophe Perignon and Yann Algan; Klaus presented the AI Overviews / publisher-revenue project in a 10-minute slot). No `*`, he presented it himself. Front position per the page's newest-first-within-year convention; it postdates SAMS (September 2026)
- **Reconciled against `miller_cv-2026-09-29a.docx` before adding anything else:** every other 2026 conference in the CV was already on the page (SAMS, Marketing Science, ZEW, EMAC, MGOW, Marketing Dynamics, Digital Economics Workshop Athens, INSEAD-HEC-ESSEC, Next Gen Antitrust/USC Gould, TU Muenchen, Bucharest, DICE, POMS). Oxera (April 2026) and INMA (June 2026) are already under Selected Invited & Industry Talks. So AI@HEC was the only gap
- The CV marks several of these 2026 entries "(planned)"; the website lists them plainly. That is a standing KM decision from June 2026 ("Includes planned 2026 talks per KM"), left alone
- Not added: the EPRS Digital Omnibus consultation (27 October 2026) has not happened yet, and it already appears under Policy & Regulatory Engagement on `media.html`

### October 2026 - Three New Policy/Litigation Citations Added
- **Bundeskartellamt, Apple ATT proceedings (B7-54-25), 13 Aug 2026, p.25 n.34** - cites "Laub, R., Miller, K. M., & Skiera, B. (2024), The Economic Value of User Tracking for Publishers, arXiv preprint arXiv:2303.10906". Added at the TOP of Policy & Regulatory Citations (reverse-chronological). **Personally re-verified**: 166pp, md5 `9b44837ecb9147e1545e8c0438c21b19`, exactly one "Miller" hit. It is the Zusagen/commitments document, hence the neutral title "Decision in the Apple App Tracking Transparency Proceedings". **It cites the arXiv version** - a concrete argument for shipping the arXiv links (open defect #3)
- **Zeithammer declaration, 2025** (`...cand.375820.778.8.pdf`), added to Cited in Litigation above the 2023 report already there. Verified: p.22 n.41 and p.23 n.45
- **Eighth Circuit amicus brief**, Internet and Consumer Law Professors supporting the FTC, March 2025, *Custom Communications v. FTC*. Verified at p.23 (body text) and p.6 (table of authorities). **It cites the paper by title as a Becker Friedman Institute working paper and never names the authors** - a name-only grep returns zero hits and would wrongly call it a false positive
- **CNIL concept paper "RGPD : quel impact economique ?" (Oct 2025) NOT added** - cnil.fr returns HTTP 503 to curl (3 attempts, browser UA + Referer) and to WebFetch, so it could not be independently verified. Agent-verified only. KM to open it in a browser and confirm
- **Eight sweep results rejected:** four are the already-listed FTC Negative Option Rule citation re-containerised (GPO reprint, 5th and 6th Cir. petition exhibits, 8th Cir. certified record list) - one citation, four documents; four are FTC PrivacyCon material, excluded by the standing July 2026 decision limiting this section to the regulator's own citing text

### October 2026 - CNIL Concept Paper, noyb Response, and an Attribution Fix
- **CNIL, "GDPR: What Economic Impact? - Concept Paper", Oct 2025** added to Policy & Regulatory Citations (cites the GDPR-on-Online-Tracking paper, p.3). **Never machine-verified**: `cnil.fr` returns HTTP 503 to curl and WebFetch. KM confirmed the document and explained the site is under maintenance - added on his say-so, not on a verification
- **noyb (European Center for Digital Rights) response to the ICO "consent or pay" call for views, 16 Apr 2024** added. Verified: endnote xxxv, p.8, citing Pay-or-Tracking Walls ("99% of users choose to accept rather than pay ... revenue increase of 16.4%")
- **ATTRIBUTION FIX, worth knowing.** The ICO entry already on the page was credited to "UK Information Commissioner's Office (ICO)". It is **not** an ICO document - it is a **joint academic submission by Utrecht University, Chalmers University and Karlstad University**, citing the paper at p.3 n.7. The filename `...-corp-cfv-reply-uk-dpa_redacted.pdf` is misleading; only opening the PDF reveals the authors. Both ICO entries now read "Response to the ICO Call for Views ..." with the **responding organisation named**
- **KM's framing for this section (2026-10-15):** these entries are "about different organizations using our research", so the responding body is the information that matters, not the consultation host. Apply that when adding future consultation responses
- Section order unchanged, reverse-chronological: Bundeskartellamt Aug 2026, AGCM Dec 2025, CNIL Oct 2025, EC Apr 2025, FTC Oct 2024, OECD Jun 2024, Utrecht/Chalmers/Karlstad 17 Apr 2024, noyb 16 Apr 2024, CNIL study Feb 2024

### October 2026 - Research Page: Abstracts, arXiv, SSRN and Data Links PUBLISHED
- Every paper now has a collapsible `<details>` abstract plus a `.paper-links` row. **9 arXiv links, 13 SSRN links, 1 Data & Code link.** This closes long-standing open defect #3 ("nine arXiv preprints exist; none are linked from research.html")
- This work had been sitting **uncommitted on disk from another session since at least 2026-10-15 morning**; KM asked about it twice before it was published
- **JEL title link restored to the AEA article page.** The uncommitted draft had reverted it to SSRN, against the 2026-09-11 decision that every Published & Accepted title links to its publisher. Verified afterwards: no Published & Accepted title points at SSRN. The SSRN preprint remains reachable from that entry's links row
- **All 9 arXiv ids verified against the arXiv API** before publishing - each resolves to the paper it sits under. Two flagged as title mismatches are the same work under preprint vs published titles: `2005.06840` ("...Ad Blockers **Affect** News Consumption?" vs "Impact") and `2411.11589` (full "General Data Protection Regulation" vs "GDPR"). No SSRN id already on the page changed; 6 were added
- `style.css` gains the `.paper-links` rules (flex row, `<details>` summary with a disclosure triangle, quoted-abstract styling)
- **Relevance:** the Bundeskartellamt's Apple ATT decision cites the **arXiv** version of the tracking-value paper, so these links are the ones regulators actually reach

### October 2026 - "Media" Renamed to "Impact"
- Nav label on all 7 pages, the `<h1>` and the `<title>` now read **Impact** (KM, 2026-10-15). Nav: Home | Research | Talks | Awards | Teaching | **Impact** | Contact
- **The filename is still `media.html`.** Deliberate: renaming it would break every existing link from the CV, papers, bookmarks and the old Google Sites redirect, and GitHub Pages has no server-side redirects. If KM ever wants `impact.html`, do it with a `media.html` meta-refresh stub left in place
- Intro rewritten to lead with the regulatory citations: "Citations of my research by regulators, competition authorities and courts, policy consultations, and press coverage:" (was "Selected media appearances, press coverage, consultations, and citations by policymakers and regulators:")
- **Reasoning:** the page holds 9 regulatory citations, 1 policy consultation, 3 court filings and 41 press entries. A tenure committee, dean or grant panel reads "Media" as press clippings and skips the strongest evidence on the site. Section order already puts policy above press, so the internal structure does the separating
- **Considered and rejected for now: splitting into two pages.** That would be an 8th nav item right after KM dropped the header title line as "heavy", and 13 policy entries are thin for a standalone page. Revisit when the policy list is longer

### October 2026 - Media Sweep: 2 New Press Items, 5 URL Fills
Six parallel search agents swept English, German, French, ad-tech trade, tech-policy/legal and institutional press. **Headline: almost no new press coverage exists.** The trade and mainstream press have covered his findings far less than the volume of regulatory citation would suggest. The sweep's real value was fixing links.
- **Added:** **noyb "Pay or Okay Report 2025"** (July 2025) - builds its central economic argument on Pay-or-Tracking Walls, reproduces "TABLE 1: ADAPTED FROM THE RESEARCH BY MULLER-TRIBBENSEE ET AL., PAGE 38", cites it in 7 footnotes. **Cites by surname only** ("Muller-Tribbensee, Miller and Skiera"), so a first-name search misses it - see [[learn_grep_title_not_author_when_verifying_citations]]
- **Added:** **CPI TechREG Chronicle** (pymnts.com, July 2024) - "A recent study by Professors Kinshuk Jerath and Klaus Miller...", with his full HEC/Hi!PARIS affiliation in the author note. This is the **original venue**; Cornerstone Research republished the same text in August 2024, so both are listed
- **5 URL fills, all source-verified:** AdExchanger, DataGrail, Cornerstone Research (name appears **only in the PDF**, not the HTML landing page), S&P Global 2018, Into the Minds 2017
- **S&P Global:** the snl.com original is **dead**. Linked to the full-text copy in Goethe's press archive. Flag for KM: that is an archive, not the publisher
- **4 entries remain unlinked:** Knowledge@HEC (GDPR tracking 2025), HBR "Cookies Are Worth More Than You Think", Law.com, Planung & Analyse Online 2017
- **DATA-QUALITY FLAG on the HBR entry:** `hbr.org/2024/11/cookies-are-worth-more-than-you-think` **404s**, and the official Nov-Dec 2024 issue TOC does not list it. Either it is print-only with no web counterpart, or **the citation itself is wrong**. Worth checking against the physical issue
- **Law.com:** the likely piece is "Academics Shower FTC With Ideas on Where Privacy Enforcement Should Head" (7 Mar 2024). Law.com's own index returns **zero** results for "Klaus Miller" and for "Skiera", so it probably credits Mueller-Tribbensee only. Verify behind the paywall before linking
- **Not added, KM's call:** a 2022 **Forbes/HEC column bylined by Klaus himself**; the ARF "Beyond Clicks" summary (names no author); a Goethe Business School blog post he wrote in 2020; Hi! PARIS and Goethe department pages (institutional, not press)
- **Coverage NOT ruled out:** search crawlers are blocked by FT, WSJ, NYT, Guardian, Economist, Politico, Euractiv, Ars Technica, The Verge, 13 of 22 French domains, and the agents' shared search budget ran out. **A Factiva/Nexis sweep via the HEC library is the only way to close this.** Also untested: Nieman Lab, MarTech, Adweek, Ad Age, Campaign, eMarketer
- **Lead worth chasing:** A Media Operator, "Few Readers Pay for Cookie-Free Site Access - but Offering the Choice May Boost Revenue" (8 Jan 2026) restates the paper's three findings in its headline but sits behind a registration wall

### October 2026 - Resting Papers Section; PUR Co-Author List Confirmed
- New **"Resting Papers"** section on `research.html`, between Working Papers and Industry Publications (KM, 2026-10-15). One entry: "How Much Ad Viewability is Enough? The Effect of Display Ad Viewability on Advertising Effectiveness", with Christina Uhl, Nadia Abou Nabout; "Working paper, 2020". Title links to SSRN 3680492; links row = Abstract, SSRN, arXiv `2008.12132`. SSRN and arXiv abstracts are identical (posted Aug/Oct 2020, never revised); arXiv's `75\%` LaTeX escape fixed to `75%`
- **Pay-or-Tracking Walls keeps Reinhold Kesler** as a co-author (KM, 2026-10-15), although SSRN 4749217 and arXiv 2403.03610 list only Müller-Tribbensee, Miller, Skiera. The site's four-author list is deliberate, not drift
- **Open, KM's call: the JEL title link 404s.** `aeaweb.org/articles?id=10.1257/jel.20261837` returns "Not Found (#404)" (checked 2026-10-15 in Chrome and by curl; the AER page answers 200, so it is not a block). The paper is also off the JEL forthcoming list and has no Crossref record yet. The link was kept on AEA by the publish commit on principle (publisher links for published entries); options are SSRN until AEA restores a page, or leave as is

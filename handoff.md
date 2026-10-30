# Website publication handoff

This checklist tracks the work needed to bring Andrea Vismara’s website to a publishable state. Update it as work is completed: mark tasks `[x]`, record relevant decisions or verification results, and add newly discovered work.

Last updated: 2026-10-30

## Current state

- Static, single-page website in `index.html`, with inline CSS and JavaScript.
- Biography, corrected affiliations, four institutional logos, public contact/profile links, portrait, and current CV are implemented.
- Publications contains four primary entries and a separate subsection with four non-first-author papers.
- Projects contains two research paper cards and the Global Remittances and Disasters Atlas, crediting Yi Zhe Ang and supervisor Liuhuaying Yang.
- Talks & Conferences still contains two placeholder entries; this is the remaining missing content section.
- Website changes through commit `af10067` have been pushed to `origin/main`. Successful deployment of the latest version and live-site behavior have not yet been verified.
- Source, local asset existence, logo file validity, and whitespace checks have been performed. Desktop/mobile browser review remains outstanding.
- Untracked `assets/CV_2025_vismara.pdf` and `assets/desktop.ini` were intentionally excluded from commits; preserve or clean up deliberately.

## Next actions, in order

1. Add real Talks & Conferences entries or hide the section and its navigation link.
2. Have Andrea review the new About biography.
3. Finish accessibility, favicon, sharing metadata, footer year, and README.
4. Complete publication/PDF checks and desktop/mobile visual review, especially logos and long titles.
5. Verify GitHub Pages deployment and all primary actions on the live site; record results below.

## 1. Confirm essential content

Completed input form: [content-input.md](content-input.md). Its answers have been applied; biography review remains open.

- [x] Apply Andrea's confirmed research introduction, current roles, and affiliation dates from the input form and subsequent ECB correction.
- [x] Confirm the preferred public email address and replace the example email link.
- [x] Replace the placeholder GitHub, Google Scholar, ORCID, and LinkedIn URLs with user-confirmed profiles; remove profiles that should not be shown.
- [x] Confirm the current public CV and update both download links to `assets/AV-CV-28102026.pdf`.
- [x] Review the wording and consistency of headings, research terminology, and contact invitation.
- [x] Resolve the ECB date discrepancy: Andrea confirmed February 2023–May 2024, inclusive; corrected the site and input form.
- [ ] Review the new CV-based About biography. Other affiliation dates were applied from the edited input table: CSH 2024, University of Vienna 2026, IIASA 2024.

Contact URLs match the supplied answers; external availability and browser interaction checks remain part of final verification.

Completion criteria: all visible personal information is accurate, and all contact and CV actions work.

## 2. Resolve projects and talks

- [x] Add three public projects: aid/debt/remittances, disaster-driven remittances, and the credited interactive atlas.
- [x] Replace project titles, descriptions, tags, and placeholder links with real content and the corresponding arXiv links.
- [x] Remove thumbnail placeholders from the two text-based project cards.
- [x] Remove unused project placeholders, including the stale reference to a “2024 publication”.
- [ ] Collect and add actual talk/conference dates, titles, events, locations, and optional slides or recordings.
- [ ] If talk details are unavailable, hide Talks and its navigation link and adjust section numbering. Projects is ready to retain.
- [ ] Search the entire page for remaining sample text, dummy profiles, and `href="#"` links.

Completion criteria: every displayed entry is substantive and accurate; no placeholder content remains.

## 3. Verify publications and downloads

- [x] Check the two research project papers and four co-authored entries against their arXiv pages for titles, author order, preprint years, and identifiers.
- [ ] Finish verification of the primary publication entries, including journal author order, venue/status, and report contribution; reconcile any CV discrepancies with authoritative sources.
- [ ] Verify every DOI, arXiv, and publisher link.
- [ ] Open each local publication PDF and confirm that it matches its entry and is suitable for public distribution.
- [ ] Check the WorldRiskReport chapter destination: the description names printed page 34, while the link uses `#page=19`; determine the correct PDF page before changing it.
- [x] Verify local existence of referenced portrait/PDF assets and validity of all four logo files.
- [ ] Verify that the portrait, logos, and every linked asset resolve on the deployed site using the exact filename and case.
- [ ] Verify both CV download links and all publication open/download actions.

Completion criteria: every publication entry and document link leads to the intended work.

## 4. Review layout and accessibility

- [ ] Render and inspect the page at desktop, tablet, and narrow mobile widths.
- [ ] Check navigation fit, long publication titles, affiliation dates, contact buttons, and horizontal overflow.
- [ ] Review portrait proportions and cropping at each layout size.
- [ ] Inspect all four affiliation logos for readability, preserved proportions, spacing, and mobile layout.
- [ ] Add and maintain `aria-expanded` and `aria-controls` for the mobile menu button.
- [ ] Verify mobile-menu opening, closing after link selection, keyboard operation, and focus visibility.
- [ ] Add a main-content landmark and a keyboard-accessible skip link.
- [ ] Add anchor scroll offsets so the sticky header does not obscure section headings.
- [ ] Check heading hierarchy, link labels, decorative SVG handling, text contrast, and image alternative text.
- [ ] Verify reduced-motion behavior and that essential content remains accessible if JavaScript is unavailable.
- [ ] Check browser console and network errors; resolve issues affecting the site.

Completion criteria: the page is readable and navigable with keyboard and touch, without broken layouts at the tested widths.

## 5. Prepare repository and publication metadata

- [x] Establish repository `Vismara-Andrea/Vismara-Andrea.github.io`, branch `main`, and push access for collaborator `AndreaVisma`.
- [ ] Confirm GitHub Pages source/settings, latest deployment success, and the live URL `https://vismara-andrea.github.io/`.
- [ ] Add a favicon.
- [ ] Review the page title and description; add the canonical URL and social-sharing metadata, including a suitable preview image.
- [ ] Update the footer copyright year.
- [ ] Replace the placeholder README with local preview, content maintenance, and deployment instructions.
- [x] Commit and push the current CV, portrait, publication PDFs, logos, and their source record with the page changes.
- [ ] Add ignore rules for incidental files such as `desktop.ini`; decide whether to retain the unused old CV locally and whether tracked `assets/trial.csv` serves any purpose.
- [ ] Confirm that no private, temporary, or unintended files are included in the publication changes.

Completion criteria: a clean checkout contains the full site and its assets, with clear instructions for maintaining and publishing it.

## 6. Final checks and launch

- [ ] Run a final placeholder, internal-anchor, local-asset, and external-link check.
- [ ] Complete a final desktop/mobile and keyboard review of the release candidate.
- [ ] Review the final content and changes with Andrea, resolving any outstanding factual or editorial decisions.
- [x] Commit and push the implemented content and assets through `af10067`.
- [ ] Commit and push the remaining finishing changes after review.
- [ ] Verify that the GitHub Pages workflow successfully publishes the final release commit.
- [ ] Verify the live URL, HTTPS, navigation, portrait, contact links, CV, and publication PDFs.
- [ ] Check the live page’s title, description, favicon, canonical URL, and sharing metadata.
- [ ] Record the release URL, date, verification results, and any deferred improvements below.

Completion criteria: the public site loads correctly and all primary actions work on the deployed version.

## Decisions and scope

- Retain About, Affiliations, Publications (including co-authored papers), Projects, and Contact.
- Talks requires real entries or removal from the visible page before the final release.
- Retain the existing visual direction and static setup unless review reveals a concrete reason to change them.

## Completion log

- 2026-10-30: Reconciled this checklist with the implemented page and successful pushes. Separated completed implementation from outstanding biography review, Talks content, technical polish, and deployment/browser verification.
- 2026-10-30: Replaced the four affiliation abbreviations with locally hosted institutional logos. Added source records in `assets/logos/README.md` and adjusted desktop/mobile logo columns to preserve the full marks. Visual browser review remains pending.
- 2026-10-29: Added a Co-authored publications subsection with the four non-first-author papers from the updated CV. Checked titles, author order, initial preprint years, and arXiv identifiers against the arXiv pages; included abstract and PDF links. Listed these as preprints without presenting submission venues as accepted publications.
- 2026-10-29: Added the Global Remittances and Disasters Atlas to Projects. Verified its title, link to the remittances paper, and visualization credits from the website's public About content: created by Yi Zhe Ang, supervised by Liuhuaying Yang.
- 2026-10-29: Added two research project cards based on arXiv:2608.21843 and arXiv:2512.16373, with descriptions checked against their abstracts and direct paper links. Removed the remaining project placeholder cards and thumbnail boxes. Talks remain unfinished.
- 2026-10-29: Andrea confirmed the ECB role ran from February 2023 through May 2024, inclusive. Updated the displayed dates and resolved the discrepancy.
- 2026-10-29: Applied the completed input form: updated the hero role, affiliation dates, public email and four profile links, and both CV links. Wrote a short About biography using the updated CV. Retained the approved introduction, headings, contact invitation, and spelling conventions. ECB date discrepancy and biography review remain open.
- 2026-10-29: Added `content-input.md` with current essential content and fields for corrections, public contact/profile links, and CV confirmation. Awaiting answers before updating the site.
- 2026-10-29: Reviewed source structure and asset inventory; created the publication checklist. No rendered or live-site verification completed yet.

## Release record

- Expected public URL: https://vismara-andrea.github.io/ (live verification pending)
- Latest pushed commit: `af10067` — Add institutional logos to affiliations
- Final release date: pending completion of remaining work
- Verification results: local source/asset checks completed; latest deployment, rendered layouts, live links, and download behavior remain unverified
- Deferred improvements: none recorded

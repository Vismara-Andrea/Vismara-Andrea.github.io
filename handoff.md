# Website publication handoff

This checklist tracks the work needed to bring Andrea Vismara’s website to a publishable state. Update it as work is completed: mark tasks `[x]`, record relevant decisions or verification results, and add newly discovered work.

Last updated: 2026-10-29

## Current state

- Static, single-page website in `index.html`, with inline CSS and JavaScript.
- Biography, affiliations, four publication entries, portrait, and local PDFs are present.
- Projects, talks, and contact/profile links still contain placeholders.
- Source and asset inventory reviewed; rendered layout, external links, and deployment have not yet been verified.
- Existing local changes predate this checklist. Preserve them while completing the site.

## 1. Confirm essential content

Input form: [content-input.md](content-input.md). Fill in the answers there; the tasks below remain open until the information is applied to the site and checked.

- [ ] Confirm the biography, research description, current roles, and affiliation dates.
- [x] Confirm the preferred public email address and replace the example email link.
- [x] Replace the placeholder GitHub, Google Scholar, ORCID, and LinkedIn URLs with user-confirmed profiles; remove profiles that should not be shown.
- [x] Confirm the current public CV and update both download links to `assets/AV-CV-28102026.pdf`.
- [x] Review the wording and consistency of headings, research terminology, and contact invitation.
- [x] Resolve the ECB date discrepancy: Andrea confirmed February 2023–May 2024, inclusive; corrected the site and input form.
- [ ] Review the new CV-based About biography. Other affiliation dates were applied from the edited input table: CSH 2024, University of Vienna 2026, IIASA 2024.

Contact URLs match the supplied answers; external availability and browser interaction checks remain part of final verification.

Completion criteria: all visible personal information is accurate, and all contact and CV actions work.

## 2. Resolve projects and talks

- [x] Decide which projects are ready for public presentation: aid/debt/remittances and disaster-driven remittances, as requested by Andrea.
- [x] Replace project titles, descriptions, tags, and placeholder links with real content and the corresponding arXiv links.
- [x] Remove thumbnail placeholders from the two text-based project cards.
- [x] Remove unused project placeholders, including the stale reference to a “2024 publication”.
- [ ] Collect and add actual talk/conference dates, titles, events, locations, and optional slides or recordings.
- [ ] Hide Projects or Talks if its content is not ready, removing the corresponding navigation link and adjusting section numbering.
- [ ] Search the entire page for remaining sample text, dummy profiles, and `href="#"` links.

Completion criteria: every displayed entry is substantive and accurate; no placeholder content remains.

## 3. Verify publications and downloads

- [ ] Verify publication titles, author names/order, years, venues, identifiers, and current publication status against authoritative sources.
- [ ] Verify every DOI, arXiv, and publisher link.
- [ ] Open each local publication PDF and confirm that it matches its entry and is suitable for public distribution.
- [ ] Check the WorldRiskReport chapter destination: the description names printed page 34, while the link uses `#page=19`; determine the correct PDF page before changing it.
- [ ] Verify that the portrait and every linked asset resolve using the exact deployed filename and case.
- [ ] Verify both CV download links and all publication open/download actions.

Completion criteria: every publication entry and document link leads to the intended work.

## 4. Review layout and accessibility

- [ ] Render and inspect the page at desktop, tablet, and narrow mobile widths.
- [ ] Check navigation fit, long publication titles, affiliation dates, contact buttons, and horizontal overflow.
- [ ] Review portrait proportions and cropping at each layout size.
- [ ] Add and maintain `aria-expanded` and `aria-controls` for the mobile menu button.
- [ ] Verify mobile-menu opening, closing after link selection, keyboard operation, and focus visibility.
- [ ] Add a main-content landmark and a keyboard-accessible skip link.
- [ ] Add anchor scroll offsets so the sticky header does not obscure section headings.
- [ ] Check heading hierarchy, link labels, decorative SVG handling, text contrast, and image alternative text.
- [ ] Verify reduced-motion behavior and that essential content remains accessible if JavaScript is unavailable.
- [ ] Check browser console and network errors; resolve issues affecting the site.

Completion criteria: the page is readable and navigable with keyboard and touch, without broken layouts at the tested widths.

## 5. Prepare repository and publication metadata

- [ ] Confirm the intended public URL and GitHub Pages deployment source/settings.
- [ ] Add a favicon.
- [ ] Review the page title and description; add the canonical URL and social-sharing metadata, including a suitable preview image.
- [ ] Update the footer copyright year.
- [ ] Replace the placeholder README with local preview, content maintenance, and deployment instructions.
- [ ] Review existing Git changes, including the moved CV, and include all required portrait/PDF assets in the release.
- [ ] Exclude incidental files such as `assets/desktop.ini`; review whether `assets/trial.csv` serves any purpose.
- [ ] Confirm that no private, temporary, or unintended files are included in the publication changes.

Completion criteria: a clean checkout contains the full site and its assets, with clear instructions for maintaining and publishing it.

## 6. Final checks and launch

- [ ] Run a final placeholder, internal-anchor, local-asset, and external-link check.
- [ ] Complete a final desktop/mobile and keyboard review of the release candidate.
- [ ] Review the final content and changes with Andrea, resolving any outstanding factual or editorial decisions.
- [ ] Commit the reviewed site and all required assets.
- [ ] Publish through the confirmed GitHub Pages workflow.
- [ ] Verify the live URL, HTTPS, navigation, portrait, contact links, CV, and publication PDFs.
- [ ] Check the live page’s title, description, favicon, canonical URL, and sharing metadata.
- [ ] Record the release URL, date, verification results, and any deferred improvements below.

Completion criteria: the public site loads correctly and all primary actions work on the deployed version.

## Decisions and scope

- Recommended first-release core: About, Affiliations, Publications, and Contact.
- Include Projects and Talks when their content is ready; their inclusion is still to be decided.
- Retain the existing visual direction and static setup unless review reveals a concrete reason to change them.

## Completion log

- 2026-10-29: Added the Global Remittances and Disasters Atlas to Projects. Verified its title, link to the remittances paper, and visualization credits from the website's public About content: created by Yi Zhe Ang, supervised by Liuhuaying Yang.
- 2026-10-29: Added two research project cards based on arXiv:2608.21843 and arXiv:2512.16373, with descriptions checked against their abstracts and direct paper links. Removed the remaining project placeholder cards and thumbnail boxes. Talks remain unfinished.
- 2026-10-29: Andrea confirmed the ECB role ran from February 2023 through May 2024, inclusive. Updated the displayed dates and resolved the discrepancy.
- 2026-10-29: Applied the completed input form: updated the hero role, affiliation dates, public email and four profile links, and both CV links. Wrote a short About biography using the updated CV. Retained the approved introduction, headings, contact invitation, and spelling conventions. ECB date discrepancy and biography review remain open.
- 2026-10-29: Added `content-input.md` with current essential content and fields for corrections, public contact/profile links, and CV confirmation. Awaiting answers before updating the site.
- 2026-10-29: Reviewed source structure and asset inventory; created the publication checklist. No rendered or live-site verification completed yet.

## Release record

- Public URL: pending confirmation
- Release date: pending
- Verification results: pending
- Deferred improvements: none recorded

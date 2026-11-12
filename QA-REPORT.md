# Website checks — 12 November 2026

## Passed

- All 22 sitemap/main pages opened in the local browser preview, including all 13 individual service pages.
- All 22 main pages have one H1 and loaded without observed broken images or desktop horizontal overflow.
- 928 HTML references checked across 24 HTML files (22 main pages plus two representations of the custom 404). No missing local page, image, stylesheet, script or fragment target was found.
- Every telephone link targets `tel:+447376668716` (124 references).
- Every static WhatsApp link targets `https://wa.me/447376668716` (92 references).
- Email links target `mailto:remapworksuk@gmail.com`.
- The footer credit uses the requested `https://www.themarketinglabdigital.com/` URL with secure new-tab attributes.
- All 13 service image files are distinct, valid WebP images, with approximately 16:9 proportions. Below-the-fold images use lazy loading.
- Every main page checked at a 320px frame width; no horizontal overflow found. Homepage additionally checked at 375, 390, 430, 768, 1024 and 1440px frame widths. Scrollbars reduce the content/client width within these frames.
- Mobile menu opens. Direct navigation from the menu/header to Services loads correctly. Link targets throughout the site resolve to existing pages.
- Form required-field, invalid email and invalid phone messages checked in the browser.
- Submitting without services displays an error and opens the service dropdown. A small outside-click handling issue was fixed and retested.
- Dropdown supports selecting multiple services, displays the selected count and closes with Done. All 13 choices remain available.
- Comments counter and 600-character maximum checked.
- Unit checks passed for WhatsApp international numbering, all message fields, multiple selected services, Unicode, line breaks, special-character URL encoding, invalid phone and missing-service validation. No external message was sent.
- FAQ disclosure controls open correctly.
- Custom 404 page renders correctly when requested directly.
- Sitemap contains 22 unique production-domain URLs and no ChatGPT URLs. Robots.txt points to the production sitemap.
- Page titles, meta descriptions, canonicals and parseable structured-data scripts checked.
- Visible mobile-service wording and footer credit are present on every page.
- JavaScript syntax check passed. No website JavaScript errors were observed; browser-extension metadata errors were excluded from website findings.

## Important limits

- These are local-preview and file checks. The ZIP has not been deployed into your Vercel account. Confirm routing, automatic unknown-path 404 handling, HTTPS and domain/DNS after upload.
- Phone/WhatsApp links were checked for correct targets and message construction, not by making live calls or sending messages. WhatsApp account ownership/delivery and email delivery were not tested.
- The external Marketing Lab URL is correctly configured, but its live availability could not be independently verified through the web retrieval service. No claim that it is offline is made.
- Analytics and advertising conversion IDs are intentionally absent/disabled; no real tracking or consent implementation has been verified.
- Legal policies remain review drafts requiring business confirmation. No genuine reviews were supplied.
- Performance has not been independently measured with Lighthouse/PageSpeed and no Core Web Vitals score is claimed.

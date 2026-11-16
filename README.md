# RemapWorks UK — GitHub upload package

Updated 16 November 2026. Includes every website change made in this conversation, including the latest Get Quote form and Starting from prices. Source snapshot: a2a481537a1c49366be802f5df8c2ef0c7b9fbca.

## Upload into the existing repository shown in your screenshot

1. First back up your current repository using Code > Download ZIP.
2. Extract this ZIP. Open RemapWorks-UK-Updated.
3. In GitHub open the existing remapworksuk.com repository, main branch, at its TOP LEVEL (where dist, source and vercel.json are visible).
4. Select Add file > Upload files. Drag in ALL the CONTENTS of RemapWorks-UK-Updated: the dist and source folders, FILE-CHECKSUMS.json, PAGE-URLS.txt, QA-REPORT.md, README.md and vercel.json.
5. Do not upload the ZIP itself. Do not drag the enclosing RemapWorks-UK-Updated folder. Do not open dist in GitHub before uploading. Correct paths include dist/index.html, dist/app.js, source/build.py and vercel.json.
6. Wait until every file finishes uploading, then Commit changes to main (or use your required pull-request workflow). Files at identical paths are updated and the new Extras page is added. The ZIP is below the browser upload file-count limit.
7. Open the SAME Vercel project's Deployments tab. With normal Git integration enabled, the new main commit triggers a deployment. Wait for Ready and confirm that deployment serves the production domain.
8. Reload the domain with Ctrl+F5 or in a private window and check Home, Services, Pricing and Contact. Do not change DNS or create a new Vercel project.

For this package, removed cards are removed by replacing dist/index.html and dist/services/index.html. There is no separate card file to delete. Uploading the folders alone does not remove arbitrary old files with different names. Existing standalone service URLs have intentionally been retained, as in the approved preview, to avoid broken links; removing a card was not a request to delete its page. They are not reintroduced as cards. If you want old service pages retired as well, that is a separate redirect/consolidation change.

If GitHub rejects the web upload, use GitHub Desktop: clone/open the same repository, copy these contents into its root choosing Replace for matching files, review changes, Commit and Push. Preserve unrelated files, custom verification tags and any manual tracking changes you added. This package reflects the preview source; it cannot include unseen edits in your GitHub repository. Back up and reconcile those before replacement.

## Vercel settings

The included vercel.json serves the already-generated dist folder with no install/build command. Framework: Other; Output Directory: dist; Root Directory: repository root. Keep your existing project/domain. Clear conflicting dashboard build/install overrides if they exist. No dependency installation is required. Existing production remains until you push and Vercel deploys successfully; no external GitHub/Vercel/DNS changes were made by this delivery.

## Included changes

- Mobile ECU remapping in Birmingham & the West Midlands; updated ECU/TCU and doorstep wording.
- Black page backgrounds, white service cards, red Call buttons, green WhatsApp buttons.
- Eight current service cards: Stage 1, Stage 2/2+, Bench ECU Remapping, Gearbox/TCU Flashing, Vehicle Diagnostics, AdBlue Diagnostics & Repair, combined DPF/EGR Solutions, Additional Services / Extras.
- Separate duplicate Performance, Economy, TCU Cloning, Software Upgrade, EGR and Swirl Flap cards stay removed. Gearbox and combined DPF/EGR were restored/grouped under later client instructions. Diesel performance/economy/50:50 choices sit within Stage 1.
- All published prices say Starting from: Stage 1 £199, Stage 2/2+ £250, Gearbox/TCU £199, all other listed services £120. Final scope and price are agreed before booking.
- Extras has its own image card, detail page, quote price and Call/WhatsApp links. Motorsport use is assessed for sound, RPM and limiter requests; road-vehicle safety/emissions systems remain intact. Swirl flap wording covers compliant diagnosis/repair.
- Compact multi-select service field. Form button says Get Quote. Form copy does not name WhatsApp; submission still prepares an encoded WhatsApp message. The customer reviews it and presses Send; opening the message is not a completed enquiry or booking.
- Footer credit: Designed By The Marketing Lab, linked to https://www.themarketinglabdigital.com/.

## Editing later

Edit source/build.py for services, prices, form options and general copy; source/enrich.py for service details. Run python3 source/build.py from the repository root, then upload/commit BOTH source and dist. Direct generated HTML edits are overwritten by regeneration. Styling: dist/style.css; form logic: dist/app.js; imagery: dist/assets. No third-party Python dependencies.

Local preview: python3 -m http.server 8080 --directory dist, then open http://localhost:8080. Form harness: node source/test-form.cjs from the repository root.

## Remaining review items

Privacy Policy and Terms are labelled review drafts, not final legal advice. Legal trading details and business terms need client review. Images are illustrative. No invented address, hours, reviews, certifications or guarantees. No analytics/advertising IDs or tags have been invented. Preserve any real tracking or verification code you added independently.

## SEO and tracking

Canonical URLs, sitemap and robots use https://remapworksuk.com only. PAGE-URLS.txt lists public page URLs. Verify the domain in Search Console and submit /sitemap.xml. Add real GA4/GTM/Ads IDs only with an appropriate consent setup and test them. A phone or WhatsApp click is not evidence of a connected call or delivered message. No live WhatsApp delivery or Google Ads conversion was claimed.

GitHub upload guide: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
Vercel Git deployments: https://vercel.com/docs/git

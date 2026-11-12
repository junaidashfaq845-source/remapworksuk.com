# RemapWorks UK — Vercel Website Package

Latest approved styling and requested revisions: black page backgrounds, white service cards, green WhatsApp buttons, red Call buttons, individual service photographs, compact multi-service enquiry dropdown, mobile-service wording on every page and The Marketing Lab footer credit.

## What to upload

Upload this entire extracted folder, including `dist/`, `source/` and `vercel.json`. The `dist` folder contains the finished HTML, CSS, JavaScript and images. No Python, Node build, database or paid dependency is required to host these finished files.

## Deploy through Vercel and GitHub

1. Extract `RemapWorks-UK-Vercel.zip` on your computer.
2. Create a GitHub repository and upload the contents of the extracted `RemapWorks-UK-Vercel` folder. `vercel.json` and `dist` must be at the repository root, not inside another wrapper folder.
3. In Vercel, choose **Add New → Project**, then import that repository.
4. Framework Preset: **Other**. Root Directory: repository root. Output Directory: **dist**. Build Command: leave empty. Install Command: leave empty. The included `vercel.json` already supplies these settings.
5. Deploy, then open the Vercel URL and check the pages listed in `PAGE-URLS.txt` before connecting your domain.

Do not upload the ZIP itself as a website file. Extract it first.

## Alternative: Vercel CLI

With Node.js installed, open a terminal in the extracted folder containing `vercel.json` and run:

```sh
npx vercel
```

Sign in and follow Vercel's prompts to create a preview. When ready to publish:

```sh
npx vercel --prod
```

No deployment or domain/DNS change has been made to your own Vercel account by preparing this package.

## Connect remapworksuk.com

In your Vercel project, open **Settings → Domains** and add `remapworksuk.com` and optionally `www.remapworksuk.com`. Use the exact DNS records Vercel displays at your domain registrar. Do not replace unrelated email/MX records. Choose one primary hostname and redirect the other to it. The current canonicals and sitemap use `https://remapworksuk.com/`.

After verification and HTTPS activation, test both hostnames, the contact form, an internal service URL and a non-existent URL. Your Vercel deployment must be checked after upload; this package has not been deployed inside your Vercel account.

## Preview locally

From the extracted project folder, with Python installed:

```sh
python -m http.server 8080 --directory dist
```

Visit `http://localhost:8080/`. Use a web server rather than double-clicking `index.html`, because asset links start at `/`.

## Edit text, prices, services and images

- Edit shared page content, contact details, service descriptions, prices and the form in `source/build.py`.
- Edit additional service-specific explanations in `source/enrich.py`.
- Rebuild the HTML from the project root with `python source/build.py`.
- Edit styles in `dist/style.css` and interactive behaviour in `dist/app.js`; these files are not overwritten by the HTML generator.
- Service photos are in `dist/assets/services/`; preserve the filenames or update the image references in `source/build.py`. Use 16:9 images. The hero is `dist/assets/hero-road.webp` and the logo is `dist/assets/remapworks-logo.svg`.
- Redeploy after editing. Never run the old one-off redesign script; it is intentionally excluded.

The supplied prices are Stage 1 from £180 and Stage 2 / Stage 2+ from £250. Other services use Request a Quote. No emission-deletion prices have been substituted for compliant repairs.

## Enquiry form

All 13 services are available through the compact multi-select dropdown on the homepage and contact page. The form validates required fields, email, phone, at least one service and consent. Comments are limited to 600 characters.

Submission prepares a URL-encoded message for WhatsApp number `447376668716`. The customer must still press **Send** in WhatsApp. Opening WhatsApp is not a confirmed enquiry, booking or conversion. No test message or telephone call was sent during checks.

## Search Console, GA4 and Google Ads

- Verify the real domain in Google Search Console using its supplied DNS verification record.
- Submit `https://remapworksuk.com/sitemap.xml` after deployment.
- Check indexing, the homepage and key service URLs with URL Inspection.
- Titles, descriptions, canonical URLs, Open Graph tags, Service/Business/Breadcrumb JSON-LD, image alt text, robots.txt and sitemap are included.
- No analytics, Google Tag Manager or Google Ads IDs are installed or invented. `window.remapWorksTracking` in `dist/app.js` is only a disabled configuration marker; filling those values alone does not install tracking.
- To enable tracking, implement the real GTM/GA4 tags and appropriate UK consent controls, then test with Tag Assistant, GA4 DebugView and the relevant Google Ads conversion diagnostics.
- Track Call/WhatsApp clicks as click events; only count qualified calls or confirmed leads as completed lead conversions when reliable measurement is available. A WhatsApp window opening is not proof of delivery.
- If the primary domain changes, update the base URL in `source/build.py` and rebuild before submission to Search Console.

## Before public launch

Privacy Policy and Terms & Conditions remain clearly marked review drafts. The business must confirm legal identity, postal contact, retention and service terms before using final policies with customers. No operating hours, physical workshop address, customer reviews, fixed performance gains or guarantees have been invented. Images are illustrative AI-generated automotive scenes, not photographs of the business premises.

See `QA-REPORT.md` for the completed checks, scope and remaining verification limits, and `PAGE-URLS.txt` for every page URL.

## Official deployment references

https://vercel.com/docs/builds/configure-a-build
https://vercel.com/docs/cli/deploy
https://vercel.com/docs/domains

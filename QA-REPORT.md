# Validation — 16 November 2026

- Latest preview source packaged at a2a481537a1c49366be802f5df8c2ef0c7b9fbca.
- 23 sitemap page URLs, with corresponding HTML files. Existing legacy service URLs intentionally remain available; their removed cards do not reappear.
- Eight service cards on Home and Services; Extras links to its new detail page.
- All referenced internal link/asset targets exist; JSON-LD parses; all price amounts carry Starting from.
- Both forms show Get Quote and omit WhatsApp in form copy; encoded WhatsApp target remains correct.
- JavaScript syntax and form harness pass, including international number, fields, Unicode/newline encoding, invalid phone and required service selection. No message sent.
- Delivered source regenerates byte-identical dist output. ZIP integrity checked.
- Earlier browser QA checked 320, 375, 390, 430, 768, 1024 and 1440px on Home, Services, Pricing and Extras with no horizontal overflow or broken loaded images. The later form-label and starting-price edits were checked in generated HTML; a fresh visual check of this package was not run.
- Your current GitHub repository and production Vercel deployment have not been changed or tested by this delivery. Check the actual deployment after upload. This package has no separate obsolete card files requiring deletion; arbitrary unknown old repository files are outside this verification.
- Legal policies remain review drafts; tracking IDs remain unconfigured. See README.

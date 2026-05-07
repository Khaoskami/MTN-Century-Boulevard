# MTN Deals - May 2026 (Mother's Day)

Static promotional landing page for MTN Century City — May 2026 Y'ello Trader.

**Validity:** 07 May – 07 June 2026

## What's new in this version
- Refreshed all deals to match the May 2026 Y'ello Trader catalogue (HONOR 600 Lite, X9d 5G, Galaxy A37/A57/S26 series, iPhone 17 family, pre-loved iPhones, AirFibre, Fibre, Sky Premium, Duo Discounts).
- **Per-deal WhatsApp buttons:** every expanded deal card now has a dedicated WhatsApp button that opens a chat with a pre-filled message in the format: *"Good day, I am contacting you about [deal] and the [price] deal."*
- **QR code:** dynamically generated on page load, pointing to the page's own URL — useful for in-store screens, printed flyers, or sharing the digital catalogue.
- Replaced the April PDF with the May Y'ello Trader (`48297_May_Consumer_Yello_Trader.pdf`).

## Deploy to Vercel
1. Push to GitHub
2. Import in [Vercel](https://vercel.com)
3. Deploy — no build config needed (`vercel.json` already points to `public/`)

## Updating for next month
The deal data lives in the `deals` array inside `public/index.html` (search for `=== DEAL DATA ===`). Edit titles, body HTML, tags, and the `msg` field (which becomes the WhatsApp pre-fill text).

## Local Preview
Open `public/index.html` in a browser. The QR code and WhatsApp links work locally too, but the QR will encode whatever local URL you're on (e.g. `file://...`) until deployed.

# Website plan

Claude keeps this file up to date so any session can pick up where the last one stopped.
Never put passwords in this file.

## Next step
Phase 4: hosting and WordPress. PAUSED by user on 2026-11-16 (deciding on paid hosting). User has NO hosting yet. Already explained: Hostinger steps + partner link, and why free hosts don't work (WordPress.com free can't install Elementor; InfinityFree-type hosts block the API connection and email for the booking form). On return: ask if they now have hosting, then Step 3 (install WordPress). (User asked about Vercel; explained it can't run WordPress; user chose WordPress. User declined Higgsfield for now.)

## Brief
- Business name: Angel's Fits (matches logo), with "Outfit Rental" as a small tagline. Facebook page is named "Angel's Outfit Rental".
- What it is, in one sentence: Cowgirl outfit rental in Mactan, Lapu-Lapu City, Cebu, Philippines.
- Facebook page: "Angel's Outfit Rental" (link not given yet)
- Real business or practice/demo site: Real business (never invent facts)
- Who it's for: Women in Cebu (Mactan / Lapu-Lapu area) needing a cowgirl, festival or party outfit for an event
- The one thing a visitor should do (call, visit, order, book, email): Fill in a booking form (event date + outfit choice)
- Pages: Home (welcome + featured outfits), Outfits (all 7 looks + what we offer), How It Works (fitting, pickup/delivery, 3-day rental, late fees, online only), Book (booking form + Facebook + hours)
- Feeling / style words: Coachella / festival theme, modern
- Colors they like or must use: Earthy desert tones (sand, terracotta, cream, brown)
- Websites they like: none given (Claude decides)
- What they already have (logo, photos, menu or price list, text):
  - content/Logo.jpg: script "Angel's" + "FITS", cowgirl hat and boots, brown on cream
  - content/Content.docx: welcome text, what we offer, location, how to rent, 3-day rental period, late fee note, online only (no physical store)
  - photos/1.png to 7.png: 7 different outfits on a mannequin, grey backdrop, small logo top-left, 1086x1448.
  - Price list: none. Site shows NO prices; use "Message us for rates" instead.
- Key facts from Content.docx: online-based, no physical store. Fittings by appointment, meet-up at LG Garden. Pickup in person or Maxim delivery. Reservations currently by Facebook DM. Rental = 3 days (pickup, event, return). Late return = extra daily fee depending on item. Offers tops, skirts, dresses, statement pieces, cowgirl hats and boots, accessories, mix-and-match. Also party outfits, not only cowgirl.
- Contact details to show (phone, email, address, hours, social links): Facebook page only ("Angel's Outfit Rental"). Available 8am to 8pm. Location: Mactan, Lapu-Lapu City (no street address; fittings by appointment at LG Garden). No phone, no email shown.
- Placeholders still waiting for real info: [FACEBOOK PAGE LINK] (exact URL). Booking form needs an inbox to receive bookings: will use the WordPress admin email (set up in Phase 4), not shown publicly.

## Design
- Direction: Golden Hour (chosen 2026-11-16). Idea: the warm last hour of light at a desert festival. Signature moments: huge Fraunces italic headlines, arch-shaped outfit photos, tilted terracotta "3-day rental" sticker, dark Mesquite band with a terracotta glow.
- Design file: design/index.html, design/outfits.html, design/how-it-works.html, design/book.html, design/styles.css
- Colors (variable name: hex): cream #FEF8EC (matches the logo's background exactly), sand #EAD9C0, terracotta #B0532C (accent/buttons), saddle #8A5532, mesquite #2B1B13 (dark bands, text), blush #E8A97F (numbers on dark)
- Fonts (heading / body): Fraunces / DM Sans
- Shared styles (class names): see design/styles.css. Key: eyebrow, eyebrow-light, section-title(-light), section-text(-light), btn-primary, btn-secondary, btn-light, btn-outline-light, btn-header, sticker, sticker-inline, section-dark, section-cta, days-grid/day-*, page-hero(-cream), page-title, footer-*
- Photo use (each once, final, user's choice 2026-11-16): Home hero arch = 5.png (White Fringe), Home "Pick a look" feature = 3.png (Denim & Fur). Outfits page = 5 looks: large arch 4.png (Look 01 Copper Corset) + 2.png, 7.png, 6.png, 1.png (Looks 02-05). User deleted the old duplicate 7.png and renamed old 8.png (Suede Fringe Set) to 7.png. How It Works and Book have no photos.
- Micro interactions (added 2026-11-16, user request): hover + transition on every button (lift) and :active press (scale 0.96); springy cubic-bezier(0.34, 1.56, 0.64, 1) wiggle on sticker, sticker-inline, feature-tag, rate-chip, header-logo, footer-logo; lift on hero-photo, feature-photo, look photos, glass-chip, day-item, note-item; slide on offer-row, step-row, footer-link; color change on faq-question, lineup-word(-alt), nav-link. All CSS hover/active + transition only (free-Elementor safe, no animation). Put each in the global class as &:hover{} / &:active{} in Phase 6.
- Trailing cursor (user request 2026-11-16): terracotta ring that follows the mouse with a soft delay, grows over links/buttons, shrinks on click. Desktop only; hidden on touch and reduced-motion. Needs JavaScript, so it is NOT built in Elementor: in Phase 7 install the free WPCode plugin and add design/cursor-snippet.html as a site-wide footer HTML snippet (ask user before installing). Preview: design/preview-cursor.html (preview only, not part of the build).
- Placeholder: Facebook link currently points to a Facebook search for "Angel's Outfit Rental"; replace with the real page URL.
- Approved on: 2026-11-16

## Photos
| File | Where it goes | Source (own photo / AI-improved / AI-made / stock) | Media ID | Source URL | Alt text |
|---|---|---|---|---|---|
| photos/5.png | Home hero arch (White Fringe) | own photo | | | Cream fringe top, white tiered skirt, tan cowgirl hat, studded belt and tall brown boots |
| photos/3.png | Home "Pick a look" feature (Denim & Fur) | own photo | | | Denim ruffle dress with belt, white fur-trim cowgirl hat and white knee-high boots |
| photos/4.png | Outfits, Look 01 Copper Corset (large arch) | own photo | | | Copper brocade corset, ruffled brown skirt, concho belt, brown hat and tall brown boots |
| photos/2.png | Outfits, Look 02 Plaid & Ruffles | own photo | | | Tied plaid shirt, white tiered skirt, studded belt, black hat and black fringe boots |
| photos/7.png | Outfits, Look 03 Suede Fringe Set | own photo | | | Tan suede fringe top and skirt set, silver concho belt, brown hat and brown boots |
| photos/6.png | Outfits, Look 04 Fringe Vest | own photo | | | Brown suede fringe vest, white tiered skirt, studded belt, brown hat and croc-print boots |
| photos/1.png | Outfits, Look 05 Golden Lace | own photo | | | Caramel lace top, white ruffle skirt, studded belt, tan hat and leopard print boots |
| content/Logo.jpg | Header and footer (logo may repeat) | own logo | | | Angel's Fits logo |
- Note: photo files are 2.3 to 2.6 MB PNGs. Before upload in Phase 6, make web JPEG copies (sips, quality 82) to keep the site fast.

## WordPress site
- Address:
- Dashboard: (address)/wp-admin
- Host and plan:
- Existing live site (it already had visitors before we started): no
  (If yes: backup first, never switch the theme, and ask before any site-wide change: site title, menu, header and footer, homepage.)
- Backup made before changes:
- Theme:
- Plugins:
- Elementor connection name (server name):
- Elementor MCP connected: no
- Atomic Editor on: unknown

## Pages
| Page | Page ID | Status (draft / published) | Edit link | Notes (sections built, with root element IDs) |
|---|---|---|---|---|

## Elementor design system
- Color variables:
- Font variables:
- Global classes:

## Site setup
- Site title and tagline:
- Homepage set:
- Menu:
- Header and footer:
- Contact form:
- Privacy Policy page (published, linked in footer):
- Search engines (demo sites: discouraged):

## Review
- First score:
- Final score:
- Open issues:

## Approvals
- 2026-11-16: Brief confirmed by user.
- 2026-11-16: Design (Golden Hour) approved by user.
- 2026-11-16: Photos approved (all own photos, no AI, no stock).

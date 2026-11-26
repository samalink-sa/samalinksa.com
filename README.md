# samalinksa.com — Sama Link website (v3, English, new visual identity)

A static one-page site for GitHub Pages. You don't need to build anything: upload the files exactly as they are.

## What changed from v2

- **New identity.** The new Sama Link logo is redrawn as a vector, using the approved colour treatments:
  - Dark backgrounds: white SAMA, bright violet LINK and symbol, off-white descriptor.
  - Deep purple backgrounds: all white.
  - White backgrounds: all deep purple.
- **Palette.** Bright Violet `#C957F9` (on dark), Deep Purple `#491375` (on white), Royal `#6F1E9E`, Plum `#3A0F63`, Night `#1A0630`, Charcoal `#0E0914`, Lavender `#F4EEF8`.
- **Font.** Kumbh Sans, self-hosted in `assets/fonts`. It's free under the Open Font License, included as `OFL.txt`.
- **Imagery** comes from the company profile: the glass S, the hand with the glass panel, the VR professional, the digital brain and the S on a cube.
- **Content** is refined from the company profile:
  - New hero subtitle.
  - Our Values section added.
  - "How we work" is now 5 steps, adding Optimise.
  - "Network Security" category, with Huawei under Networking.
  - Updated compliance wording.
  - Sama Group logo added in the hero and the footer.
- **Sharing.** A link preview image for WhatsApp and LinkedIn (`assets/img/og-image.jpg`) and a phone home-screen icon.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole site (one scrolling page, logos embedded as vectors) |
| `assets/style.css` | Styles: colours, font, layout, mobile |
| `assets/favicon.svg` | Browser tab icon (S symbol) |
| `assets/fonts/` | Kumbh Sans web font and its licence |
| `assets/img/` | Section images, share preview image and home-screen icon |
| `CNAME` | Serves the site at `samalinksa.com`. Don't delete it. |
| `404.html` | Branded "page not found" page |
| `robots.txt`, `sitemap.xml` | Let search engines find and index the site |

## Updating the live site on GitHub

1. Open the repository `samalink-sa/samalinksa.com` → **Add file → Upload files**.
2. In File Explorer, open this folder and press **Ctrl+A**. That selects the `assets` folder and all the files beside it. Drag the whole selection onto the page.
   - A file with the same name replaces the old one, and new files are added.
3. Write a commit message such as `Website v3 – new visual identity` → **Commit changes**.
4. Wait 1–2 minutes, then open https://samalinksa.com and press **Ctrl+F5**.

## Common changes

- **Contact form.** It opens the visitor's email app, with the message addressed to `info@samalinksa.com`. To collect replies in Microsoft 365 instead:
  1. Create a form in Microsoft Forms.
  2. Choose **Collect responses → Embed** and copy the `<iframe>`.
  3. In `index.html`, replace the `<form class="form" id="contact-form"> … </form>` block with that iframe.
- **Arabic version.** Planned as `ar/index.html` (RTL), with a language switch in the header.

## Content rules this site follows

These come from the company profile:

- AI & Business Automation leads as our edge.
- Managed IT covers M365 & user admin, Intune devices & patching, Windows Server & AD, and proactive support.
- No client names, no partnership claims, no SLA numbers and no 24/7 promises.
- Vendors appear as plain text, with the trademark note.
- The Vision 2030 logo, the national emblem and the Saudi flag are deliberately not used on the site. Each has its own official usage rules.

# samalinksa.com — Sama Link website (v2, English)

A static one-page site, ready for GitHub Pages. You don't need to build anything: upload these files exactly as they are.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole site (one scrolling page) |
| `assets/style.css` | Styles: brand colours, Sora + Inter fonts, mobile layout |
| `assets/favicon.svg` | Browser tab icon (S mark) |
| `CNAME` | Tells GitHub Pages to serve the site at `samalinksa.com` |
| `404.html` | Branded "page not found" page |
| `robots.txt`, `sitemap.xml` | Let search engines find and index the site |

## Publish on GitHub Pages

1. Create a free GitHub account with the company email, then create a **public** repository (for example `samalinksa.com`).
2. In the repository: **Add file → Upload files**. Drag in the contents of this folder (the `assets` folder too, not the folder that contains everything), then **Commit changes**.
3. **Settings → Pages**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`, then **Save**.
4. In the same page, under **Custom domain**, check that `samalinksa.com` is filled in (the `CNAME` file does this) and save.
5. In the **Microsoft 365 admin center → Settings → Domains → samalinksa.com → DNS records → Custom records**, add:
   - `A  @  185.199.108.153`
   - `A  @  185.199.109.153`
   - `A  @  185.199.110.153`
   - `A  @  185.199.111.153`
   - `CNAME  www  <your-github-username>.github.io`

   **Do not touch the existing email records** (MX, autodiscover, SPF and so on).
6. Wait for GitHub's DNS check to pass and the certificate to be issued (up to about an hour), then tick **Enforce HTTPS**.
7. Test `https://samalinksa.com` and `https://www.samalinksa.com` on a laptop and a phone.

## Updating the site later

Edit a file on GitHub (pencil icon) or upload a replacement file with the same name. The site updates within a minute or two.

## Common changes

- **Sama Group logo.** Once the official vector arrives, save it as `assets/sama-group-logo.svg`. Then add `<img src="assets/sama-group-logo.svg" alt="Sama Group of Companies" height="40">` where the comment in the hero section of `index.html` marks it.
- **Contact form.** Today the form opens the visitor's email app, with the message addressed to `info@samalinksa.com` and ready to send. No server is needed. To collect replies in Microsoft 365 instead:
  1. Create a form in Microsoft Forms.
  2. Choose **Collect responses → Embed** and copy the `<iframe>` code.
  3. In `index.html`, replace the `<form class="form" id="contact-form"> … </form>` block with `<div class="form"> PASTE IFRAME HERE </div>`.
- **Arabic version.** Planned after English sign-off, as `ar/index.html` (RTL, IBM Plex Sans Arabic) with a language switch in the header.

## Content rules this site follows

These come from the company profile. Keep them when you edit:

- AI & Business Automation leads as our edge.
- Managed IT covers M365 & user admin, Intune devices & patching, and Windows Server & AD only. No monitoring, helpdesk or backup.
- No Odoo ERP and no cybersecurity line for now.
- No client names, no partnership claims, no SLA numbers and no 24/7 promises.
- Vendors appear as plain text, with the trademark note.

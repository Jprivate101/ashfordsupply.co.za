# ashfordsupply.co.za

The public website for Ashford Supply Co (Appreciation Company (Pty) Ltd t/a Ashford Supply Co).
Plain HTML and CSS, hosted free on GitHub Pages. No build step, no framework, nothing to install.

## What is where

| File | What it is |
|---|---|
| `index.html` | The homepage. Each section is marked with a comment (HERO, VALUES, ABOUT, CONTACT + QUOTE FORM). |
| `thanks.html` | Shown after someone sends the quote form. |
| `404.html` | Shown for any broken link. |
| `styles.css` | Every colour, font and layout rule. Brand colours are at the top in `:root`. |
| `assets/` | Logo, truck photo, favicon, social share image (`og-image.jpg`, 1200 x 630). |
| `CNAME` | Tells GitHub Pages the site lives at ashfordsupply.co.za. Do not delete. |
| `robots.txt`, `sitemap.xml` | For Google. Add any new page to `sitemap.xml`. |

## Brand

- Navy `#0F2D4A`, Brass `#C9A227`, Off-white `#F7F5EF`
- Headings: Libre Baskerville (serif). Body: Outfit (sans). Both from Google Fonts.
- Tagline: Value · Reliability · Straight dealing

## Contact details used on the site

- Email: sales@ashfordsupply.co.za (forwards to Gmail)
- WhatsApp only: +27 65 205 6761, linked as `https://wa.me/27652056761?text=...`
- No call number is published on purpose.

## The quote form

Sent by [FormSubmit](https://formsubmit.co) (free, no account) to sales@ashfordsupply.co.za.

- The form `action` uses FormSubmit's private alias `52e8e9a7129ea67d041b9a583c924e56` instead of the email address, so bots cannot scrape sales@ from the page. The alias belongs to sales@ashfordsupply.co.za (activated 27 Oct 2026).
- Activation is per web address: http and https were each activated once (27 Oct 2026). If the site ever moves to a new domain, send one test enquiry and click the activation email before telling anyone, otherwise visitors see a "Check Your Email" page.
- To send enquiries somewhere else, change the action to `https://formsubmit.co/<new email>` and click the activation email FormSubmit sends on the first submission.

- Spam protection: a hidden `_honey` field. Bots fill it in and FormSubmit drops the message. No CAPTCHA.
- After sending, the visitor lands on `thanks.html` (set by the `_next` field).
- Subject line of each enquiry: "New quote request from ashfordsupply.co.za".
- If the form ever stops working, the email link under the button still works.

## How to change something

1. Edit the file (on github.com: open the file, click the pencil, then "Commit changes").
2. GitHub Pages republishes automatically within a minute or two.
3. Every change is a saved version. To undo, revert the commit.

### Add a new page

1. Copy `thanks.html` to e.g. `kimbies.html` (it already has the shared header and footer).
2. Replace the content between `<main id="main">` and `</main>`, using the section classes from `index.html` (`section`, `two-col`, `value`, `facts`, `btn btn-navy`, etc).
3. Change the `<title>` and `<meta name="description">`, and remove the `noindex` line so Google lists it.
4. Add it to the nav in the header of every page if it needs a menu link, and to `sitemap.xml`.

## DNS (at domains.co.za)

- `ashfordsupply.co.za` A records: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 (GitHub Pages)
- `www` CNAME: jprivate101.github.io
- Mail records (MX, `mail`, `webmail`, SPF, DKIM, DMARC) are separate. Do not touch them when changing the website.

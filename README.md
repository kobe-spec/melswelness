# Mel's Wellness — website

618 Chestnut Rd STE 203, Myrtle Beach, SC 29572 · (843) 450-9051

No folders. Every file sits side by side, so uploading is a single drag.

## Files

```
index.html                          Home (also holds About and Contact)
services.html                       Services & pricing
reflexology.html
couples-massage.html
signature-massage.html
post-op-lymphatic-massage.html
lymphatic-drainage-massage.html
restora-pelvic-floor-chair.html
3-in-1-infrared-red-light-pemf.html
nano-vi.html
(8 image files)
robots.txt
sitemap-TEMPLATE.xml
```

## Upload to GitHub

1. Download and unzip this folder.
2. Go to github.com/new — name it `melswellness`, set **Public**, Create.
3. Click **uploading an existing file**.
4. Open the unzipped folder, press **Ctrl+A** (Mac: **Cmd+A**) to select all the files,
   and drag them onto the GitHub page.
5. Click **Commit changes**.

Because there are no subfolders now, the "choose your files" button works too — it just
can't handle folders, which is what broke the first attempt.

## Turn on GitHub Pages

Settings → Pages → Source: **Deploy from a branch** · Branch **main** · Folder **/ (root)** → Save.
Wait 1–2 minutes, then refresh that page for your link.

Test it by clicking through to a service page from the homepage menu.

## After it's live

Open `sitemap-TEMPLATE.xml`, replace every `SITE_URL` with your live address
(e.g. `https://yourname.github.io/melswellness`, no trailing slash), rename it to
`sitemap.xml`, and add to `robots.txt`:

```
Sitemap: https://yourname.github.io/melswellness/sitemap.xml
```

Send me the live link and I'll handle this.

## Adding a real domain later

Worth doing — a `.github.io` address ranks worse locally than `melswellness.com` would.
Buy the domain, then at the registrar add four `A` records for `@` pointing to
`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`, and a
`CNAME` for `www` → `<username>.github.io`. Then Settings → Pages → Custom domain.

## Local SEO checklist

1. **Google Business Profile** — claim and verify at the exact address above.
   Primary category: *Massage therapist*.
2. **Link each service** — in the profile's Services section, link individual services to
   their own page (e.g. `.../reflexology.html`), not just the homepage.
3. **Google Search Console** — add the site, submit the sitemap.
4. **Citations** — name, address, phone identical everywhere (Apple Maps, Yelp, Facebook,
   massage directories). Exact formatting matters.
5. **Reviews** — ask clients to name the service and city
   ("lymphatic drainage in Myrtle Beach"). That wording feeds local ranking.
6. **Photos** — add new studio photos to the Business Profile monthly.

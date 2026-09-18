# Mel's Wellness — website

Static site for Mel's Wellness · 618 Chestnut Rd STE 203, Myrtle Beach, SC 29572 · (843) 450-9051

## What's here

```
index.html                          Home (+ #about, #contact sections)
services/index.html                 Services & pricing hub
restora-pelvic-floor-chair/         \
lymphatic-drainage-massage/          |
post-op-lymphatic-massage/           |
signature-massage/                   |  One folder = one service page.
couples-massage/                     |  Each is standalone static HTML with its own
reflexology/                         |  title, meta description and Service +
3-in-1-infrared-red-light-pemf/      |  FAQPage + Breadcrumb schema.
nano-vi/                            /
uploads/                            Images used by the service pages
robots.txt                          Crawler rules
sitemap-TEMPLATE.xml                Fill in your live URL, rename to sitemap.xml
.nojekyll                           Tells GitHub Pages to serve files as-is
```

`index.html` is fully self-contained — images and scripts are embedded. The service pages
load their photos from `uploads/`. Every page uses relative links, so the site works at any
address: `yourname.github.io/repo/`, a custom domain, or a plain folder on your computer.

## Upload to GitHub

1. Create a new public repository at https://github.com/new — name it e.g. `melswellness`.
2. On the new repo page, click **uploading an existing file**.
3. Drag in **the contents of this folder** — every file and folder listed above.
   Do not drag the folder itself; `index.html` must end up at the top level of the repo.
4. Click **Commit changes**.

## Turn on GitHub Pages

1. Repo → **Settings** → **Pages**
2. Source: **Deploy from a branch** · Branch: **main** · Folder: **/ (root)** → **Save**
3. Wait 1–2 minutes. Your site goes live at `https://<username>.github.io/<repo>/`

Check that the service pages work by visiting `https://<username>.github.io/<repo>/reflexology/`.

## One step after it's live

Open `sitemap-TEMPLATE.xml`, replace every `SITE_URL` with your live address
(e.g. `https://yourname.github.io/melswellness`, no trailing slash), rename the file to
`sitemap.xml`, and add this line to the bottom of `robots.txt`:

```
Sitemap: https://yourname.github.io/melswellness/sitemap.xml
```

Send me the live URL and I'll do this for you, plus bake the absolute canonical URLs in.

## Adding a real domain later

A custom domain is worth it — a `.github.io` address ranks noticeably worse for local
searches than `melswellness.com` would.

1. Buy the domain, then add DNS records at the registrar:
   - Four `A` records for `@` → `185.199.108.153`, `185.199.109.153`,
     `185.199.110.153`, `185.199.111.153`
   - One `CNAME` record for `www` → `<username>.github.io`
2. Repo → Settings → Pages → Custom domain → enter the domain → Save
3. Tick **Enforce HTTPS** once the certificate is issued (up to an hour)

## After launch — local SEO checklist

1. **Google Business Profile** — claim and verify the listing at the exact address above.
   Primary category: *Massage therapist*. Add the website URL.
2. **Link each service** — in the Business Profile's Services section, point individual
   services at their own page (e.g. `.../reflexology/`), not just the homepage.
3. **Google Search Console** — add the property, submit `sitemap.xml`.
4. **Bing Webmaster Tools** — same; it can import from Search Console.
5. **Citations** — name, address and phone must match *exactly* on Apple Maps, Yelp,
   Facebook and massage directories. Identical formatting matters.
6. **Reviews** — ask clients to name the service and the city in their review
   ("lymphatic drainage in Myrtle Beach"). That language feeds local ranking.
7. **Photos** — post new studio photos to the Business Profile monthly.

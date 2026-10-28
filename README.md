# AutoCloudX (ACX) — Marketing Site

Front-end-only marketing site for AutoCloudX: Home, Learning Paths, Labs & Projects, AI Network Mentor (demo), About, Contact.

- Content data: `src/lib/content.ts` (paths, labs), `src/lib/mentor.ts` (curated mentor answers)
- Site settings: `src/lib/site-config.ts` (domain, contact email, booking link, channels)

## Launch checklist

- [ ] **Official domain** — set `siteConfig.url`; update canonical/og:url to absolute URLs; add `Sitemap:` line in `public/robots.txt` and generate a sitemap.
- [ ] **Business contact** — set `siteConfig.contact.email` / `bookingUrl` / `channels`. Nothing is invented by default.
- [ ] **Contact form delivery** — `src/routes/contact.tsx` currently validates only (see `TODO(launch)`). Connect a server function + email provider.
- [ ] **Live AI mentor** — replace `getMentorReply` with a server-side call to an AI provider. Keep API keys server-side only; add rate limiting and update the in-UI demo notice.
- [ ] **Analytics & privacy** — add analytics (if any) plus a privacy notice / cookie consent as required.
- [ ] **Share image** — add a 1200×630 Open Graph image once the domain is known.
- [ ] **Final content review** — verify all copy, lab examples and vendor references; keep the "not official vendor certification" disclaimer.

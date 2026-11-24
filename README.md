# Ahmed-Emad-Nasr.github.io

The root of https://ahmed-emad-nasr.github.io — it only sends visitors to the
portfolio at https://ahmed-emad-nasr.github.io/ahmed.dev/ and tells crawlers
where its sitemap is.

- `index.html` / `404.html` → redirect to /ahmed.dev/
- `robots.txt` → crawlers read robots.txt only at the root of a domain
- `sitemap.xml` → sitemap index: `sitemap-root.xml` (this home page) + the
  portfolio's `/ahmed.dev/sitemap.xml`
- `.well-known/security.txt` → RFC 9116 security contact (renew `Expires`
  yearly — it is set to 23 Nov 2027)
- The numbers on `index.html` are "N+" floors that stay true as they grow;
  its `sameAs` list must match SAME_AS in the portfolio (lib/seo.ts)
- `.nojekyll` → GitHub Pages serves the `.well-known` folder

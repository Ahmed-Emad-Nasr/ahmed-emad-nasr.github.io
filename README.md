# Ahmed-Emad-Nasr.github.io

The root of https://ahmed-emad-nasr.github.io — it only sends visitors to the
portfolio at https://ahmed-emad-nasr.github.io/ahmed.dev/ and tells crawlers
where its sitemap is.

- `index.html` / `404.html` → redirect to /ahmed.dev/
- `robots.txt` → crawlers read robots.txt only at the root of a domain
- `.well-known/security.txt` → RFC 9116 security contact (renew `Expires` yearly)
- `.nojekyll` → GitHub Pages serves the `.well-known` folder

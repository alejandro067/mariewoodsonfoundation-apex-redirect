# mariewoodsonfoundation-apex-redirect

Apex redirect only. The GitHub Pages A records (185.199.108-111.153) on
`mariewoodsonfoundation.org` point here, and every request is bounced to `https://www.mariewoodsonfoundation.org`, which is
the Cloudflare Pages site.

DNS for this domain lives at Wix. This domain currently has **no MX records at all**; foundation mail is a plain Gmail address.

Both `index.html` and `404.html` carry the same redirect: GitHub Pages serves
`index.html` only for `/`, so without `404.html` every deep link into the apex
would land on GitHub's own 404 page instead of the site.

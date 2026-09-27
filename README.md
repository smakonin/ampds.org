# AMPds website redirect

The website now lives at https://makonin.com/ampds/ in smakonin/smakonin.github.io.

GitHub Pages publishes this repository from gh-pages. index.html redirects immediately using location.replace (preserving fragment anchors), with a meta-refresh fallback and a visible link when automatic navigation is unavailable. 404.html sends old missing paths to the new homepage. Existing assets and CNAME are retained.

This is a static browser redirect, not an HTTP 301/308: GitHub Pages does not provide configurable server-side redirect rules. HTTPS for the source hostname must be working before any browser redirect can run. At setup, the Pages API reported no HTTPS certificate for ampds.org.

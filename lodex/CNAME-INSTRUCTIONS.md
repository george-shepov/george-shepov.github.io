# lodex.giorgiy.org setup

The LODEX landing page currently lives at:

`https://george-shepov.github.io/lodex/`

To expose it at `https://lodex.giorgiy.org`, choose one deployment approach.

## Preferred: reverse proxy on 104.237.9.52

1. Point the DNS `A` record for `lodex.giorgiy.org` to `104.237.9.52`.
2. Serve or proxy the LODEX static page from the VPS.
3. Request a Let's Encrypt certificate for `lodex.giorgiy.org`.
4. Redirect HTTP to HTTPS.

## Alternative: GitHub Pages custom domain

GitHub Pages supports one custom domain for the entire `george-shepov.github.io` site. Configure `lodex.giorgiy.org` only if the root Pages hub should also use that host.

Do not add a nested `CNAME` file expecting it to apply only to `/lodex/`; GitHub Pages custom domains are configured per Pages site, not per subfolder.

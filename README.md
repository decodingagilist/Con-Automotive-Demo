# Cox Automotive Australia — Landing Page Demo

Single self-contained static file: `index.html`. No build step, no dependencies to install.

## Deploy on GitHub Pages (works with wordsell.com via a custom domain)

1. Create a new GitHub repo (e.g. `cox-automotive-demo`).
2. Upload `index.html` from this folder to the repo root (GitHub web UI: **Add file → Upload files**).
3. Repo **Settings → Pages** → Source: `Deploy from a branch`, branch `main`, folder `/root`. Save.
4. GitHub gives you a `https://<user>.github.io/<repo>/` URL within a minute or two.
5. To use `wordsell.com`: in the same Pages settings, add it under **Custom domain**, then at your DNS provider add a `CNAME` record for `wordsell.com` (or the subdomain you're using) pointing to `<user>.github.io`. GitHub Pages auto-provisions HTTPS once DNS propagates.

Any other static host (Netlify, Vercel, S3, Cloudflare Pages) works the same way — just point it at `index.html`.

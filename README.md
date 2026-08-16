# hudly.dev

Landing page for [Hudly](https://hudly.dev) — a visual HUD editor for Unreal Engine.

Static, dependency-free, served via GitHub Pages.

## Publish

1. Create the repo `hudly` in the `hudly-dev` org (public).
2. Push this folder:

   ```
   git remote add origin git@github.com:hudly-dev/hudly.git
   git push -u origin main
   ```

3. Repo → Settings → Pages: source "Deploy from a branch", branch `main`, root.
   The `CNAME` file sets the custom domain `hudly.dev` automatically; tick
   "Enforce HTTPS" once the certificate is issued (takes a few minutes).

## DNS (INWX, zone hudly.dev)

| Type  | Name | Value               |
| ----- | ---- | ------------------- |
| A     | @    | 185.199.108.153     |
| A     | @    | 185.199.109.153     |
| A     | @    | 185.199.110.153     |
| A     | @    | 185.199.111.153     |
| CNAME | www  | hudly-dev.github.io |

These coexist with the Proton mail records (MX/TXT) — different record types,
no conflict.

## License

© 2026 Hudly. All rights reserved. This repository is public so the site can be
served via GitHub Pages — that does not grant any right to reuse its content,
design or brand assets.

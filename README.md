# Lloyd White for Beaumont City Council

Static campaign site — plain HTML/CSS, no build step required.

## Files
- `index.html` — Home
- `about.html` — About
- `issues.html` — Issues / platform
- `donate.html` — Donate (link out to ActBlue/WinRed)
- `volunteer.html` — Volunteer sign-up form
- `yard-sign.html` — Yard sign request form
- `css/style.css` — Shared styles

## Before you launch
1. **Find/replace** every `[Your Name]`, `[Committee Name]`, and `[FPPC ID#]` placeholder across all files.
2. **Donate page**: replace the placeholder buttons with your real ActBlue or WinRed link/embed.
3. **Forms**: the volunteer and yard-sign forms point to `https://formspree.io/f/YOUR_FORM_ID`. Since this is a static site, you need a form backend to receive submissions — sign up free at formspree.io (or getform.io / basin.so), create a form, and swap in your real endpoint. Until then, submissions go nowhere.
4. **Disclaimer**: confirm exact required wording with the Riverside County Registrar of Voters or the FPPC before publishing — the footer text here is a placeholder.
5. Fill in real copy in `about.html` and `issues.html` (marked with `[...]`).

## Deploy on Cloudflare Pages
1. Push this folder to a GitHub repo.
2. In Cloudflare dashboard → Pages → Create a project → Connect to Git → select the repo.
3. Build settings: **Framework preset: None**, **Build command: (leave blank)**, **Build output directory: /** (root).
4. Deploy. Cloudflare will give you a `*.pages.dev` URL; add your own domain under Custom Domains once you have one.

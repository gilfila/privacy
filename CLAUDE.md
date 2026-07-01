# privacy

Static **Privacy Policy** (and **Terms of Service**) page for the **T1D Notifier** app. Not an application — just hand-written static HTML pages, no build step, no dependencies.

## What's here
- `index.html` — the privacy policy page (renamed from `privacy.html` so Render serves it at root). Self-contained: inline `<style>`, DM Sans / DM Serif Display web fonts. Contact is set to Tony Gilfillan / tony.gilfillan@gmail.com; "Last updated" date is 2025-03-04.
- `terms.html` — boilerplate Terms of Service page, linked from the privacy policy.
- `README.md` — Render deployment guide.

## How it's used / deployed
- Hosted as a **Render Static Site** (no build command; publish directory `.`). Render serves `index.html` at the root URL.
- Optional Render rewrite rule maps `/privacy` → `/index.html` so the page lives at `https://<site>.onrender.com/privacy`.
- Local preview: open `index.html` directly in a browser — no server needed.

## Constraints / notes
- Pure static HTML/CSS; keep it dependency-free and build-free.
- To edit the policy, change the HTML and bump the "Last updated" date, then commit + push — Render auto-redeploys.

## Last turn / Pending
- Serves the **T1D Notifier** app (privacy policy + terms). Deployed on Render; the `/privacy`
  rewrite rule maps to `index.html`. Last content update 2025-03-04. No major pending work.
- No state/TODO files present. Last commits (per `git log`) added the Terms of Service page, the contact name/email, and the Render deployment guide — all merged. All files last modified 2025-03-04; the contact placeholder is already filled in.
- If resuming, check `git log --oneline` and recent file mtimes for the latest state.

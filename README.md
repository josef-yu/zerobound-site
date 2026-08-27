# zerobound-site

Public site for **Zerobound** — currently just the privacy policy required by the
Google Play listing. The game's source lives in a separate **private** repo; this
repo is intentionally public so GitHub Pages can serve the policy on the free plan.

## What's here
- `index.html` — the privacy policy (self-contained, no build step).
- `.github/workflows/deploy.yml` — GitHub Actions workflow that publishes the site to
  GitHub Pages automatically on every push to `main`.

## Publish with GitHub Pages
1. Create a **public** repo named `zerobound-site` on GitHub (empty, no README).
2. Push this folder to it (see commands below).
3. Repo **Settings → Pages → Build and deployment → Source = "GitHub Actions"**.
   (One-time. No branch/folder to pick — the workflow handles it.)
4. The `Deploy to GitHub Pages` action runs on the push and publishes in ~1 minute to:
   `https://<your-github-username>.github.io/zerobound-site/`
   Every later push to `main` re-deploys automatically.

Use that URL as the **Privacy policy** link in the Play Console listing.

Developer: **Ontex** · Contact: **ontex@josefyu.com**

## Keep it accurate
The policy states the app collects no data and has no network access. **If ads or any
network feature are added later, update `index.html` and the Play "Data safety" form
before releasing that version.**

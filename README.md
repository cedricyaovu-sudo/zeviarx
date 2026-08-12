# Zevia Rx

Direct-response telehealth GLP-1 marketing site — landing page + 2-minute eligibility
quiz with a multi-tier BNPL checkout and card soft-pivot. Static site, no build step.

## Structure
- `index.html` — landing page (hero pill animation, medications, experts, member stories, plans, FAQ)
- `quiz.html`  — eligibility quiz + checkout funnel
- `assets/`    — images (webp/jpg) and videos (mp4 + webm)
- `vercel.json`— clean URLs (so `/quiz` serves quiz.html)

## Deploy to Vercel (import this repo)
1. Push this folder to a new GitHub repo (commands below).
2. On vercel.com → **Add New → Project → Import Git Repository** → pick this repo.
3. Framework preset: **Other**. Build command: none. Output dir: leave default (root).
4. Deploy. Every future `git push` auto-deploys.

## Push to GitHub
Create an empty repo named `zeviarx` on github.com (no README/gitignore), then:

    git init
    git add -A
    git commit -m "Zevia Rx site"
    git branch -M main
    git remote add origin https://github.com/<your-username>/zeviarx.git
    git push -u origin main

## Pre-launch notes (design build)
Press logos, member reviews/photos/videos, and medical-expert profiles are **illustrative
placeholders** and carry on-page disclosures — replace with real, verified, consented
content before going live. The checkout is a front-end demo (no real payment); wire Stripe +
the BNPL provider APIs before launch.

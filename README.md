# Darken Shadows Swimming Club — Static Demo

A frontend-only, static HTML/CSS/JS conversion of the Darken Shadows Swimming Club
booking platform, built for live portfolio demos (no PHP/MySQL backend required).

**Live demo:** deploy this repo to Vercel (or open `index.html` directly).

## What this is

The original project is a full PHP/MySQL swimming club booking platform with:
- Session-based auth
- 6 dedicated program pages backed by a polymorphic `bookings` table
- A MySQL trigger generating unique booking reference codes
- An admin panel for managing enrollments

This repo is a **static demo build** of the same UI/UX, converted so it can be hosted
for free on Vercel and clicked through without a server. It is not the production app.

### What's different from the real app
- No login/session — every page renders as a logged-in "Guest" user with sample data
- No database — the Profile page shows two sample bookings and a sample membership
- Forms don't hit a real backend — submitting any enrollment/membership form shows a
  "Thanks for submitting!" confirmation with a generated demo reference number
- Admin panel, coach panel, and Facilities page are excluded from this demo
- Hero background images are placeholder gradients — swap in real photos in `images/bg/`

## Pages

| Page | File |
|---|---|
| Home | `index.html` |
| Programs (all 6) | `program.html` |
| Junior Development | `junior.html` |
| Competitive Squad | `competitive.html` |
| Elite Coaching | `elite.html` |
| Adult Fitness Swim | `adult.html` |
| Mental Conditioning | `mental.html` |
| Masters Program | `masters.html` |
| Membership | `membership.html` |
| Profile (sample data) | `profile.html` |

## Running locally

No build step needed — plain static files.

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Deploying to Vercel

1. Push this repo to GitHub.
2. Import it in [Vercel](https://vercel.com/new).
3. Framework preset: **Other** (static site) — no build command needed.
4. Deploy.

## Tech

HTML5, CSS3, vanilla JS. Fonts via Google Fonts (Cinzel + Raleway).

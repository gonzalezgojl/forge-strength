# Career 360 — Aviation Opportunities

Mobile-first job search PWA for EASA B1.1 aircraft maintenance professionals.

## Features

- Live-on-demand search against YubHub's public job search endpoint.
- Search terms: aircraft, aviation, aircraft maintenance, B1 engineer, licensed aircraft engineer and aircraft technician.
- European-region filtering and relevance score based on the saved candidate profile.
- Defaults: EASA B1.1, A350/A330/A320, Line Maintenance, Europe, €50/hour target, day shifts, accommodation/allowance and 5/5 or 7/7 rotations.
- Saved opportunities, application status and private notes stored locally.
- Direct links to source job advertisements where supplied.
- Links to LinkedIn Jobs, Aviation Job Search, JSfirm and web search.
- PWA manifest and offline shell cache.

## Live source and freshness

The app queries `https://api.yubhub.co/search` when the user taps **Comprobar ofertas ahora**. YubHub documents its read/search endpoint as public, no-key and CORS-enabled. The provider states that its listing data is refreshed at least hourly and applies a limit of 30 search requests per minute per IP. This is a live check of the available catalogue, not an instant query of every employer ATS or a guarantee that every aviation vacancy is indexed.

Data attribution: **Data by YubHub** — https://yubhub.co

## Deployment

Enable GitHub Pages from **Settings → Pages → Deploy from a branch**, branch `main`, folder `/ (root)`.

App URL:
`https://gonzalezgojl.github.io/forge-strength/career-360/`

## iPhone installation

1. Open the deployed URL in Safari.
2. Tap Share → Add to Home Screen.
3. Confirm Add.

## Privacy

Candidate preferences, saved vacancies, application statuses and personal notes are kept in local browser storage on the device. No login is needed. Vacancy searches are sent to YubHub's public API.

## Files

- `index.html` — app interface and search logic.
- `manifest.webmanifest` — PWA metadata.
- `sw.js` — offline shell cache.
- `icon.svg` — app icon.

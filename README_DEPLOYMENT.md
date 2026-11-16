# ALSKwela A&E 2027 — JHS LS2 Science Offline Reviewer

## App name
Full installed app name: **JHS ALS A&E Reviewer LS 2 - Science**  
Home Screen shortened label: **JHS A&E LS2 Science**

## Upload to GitHub Pages
1. Create a NEW GitHub repository e.g. `alskwela-ls2-science-reviewer-jhs`.
2. Extract this ZIP, then upload `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, and `.nojekyll` directly to the **root** of that repository; do NOT upload the ZIP itself.
3. GitHub → repository → Settings → Pages → Deploy from a branch → main / (root).
4. In the ALSKwela Glide App create a card with Open Link to the deployed GitHub Pages HTTPS URL.
5. Learners open the URL DIRECTLY in Chrome, confirm `Offline files saved successfully`, then install/add Home Screen. Airplane-mode test before rollout.

## Reviewer behavior
- 120 unique science multiple-choice questions, one correct choice among A-D.
- Three fixed sets of 40, each 12 Easy / 20 Moderate / 8 Challenging, with 40 different LC codes per set.
- Balanced Random 40: chooses 40 of 46 LC codes and respects 12/20/8 difficulty targets; prioritizes less-seen questions over successive trials.
- English questions; professional Taglish explanation, positive and encouraging feedback.
- Progress saved locally and PDF report made on device (optionally include explanations). Works offline after first successful caching.
- No learner account, data transmission, or teacher dashboard. Device storage can be cleared; retain PDF reports.

## Academic and data limitations
- Mock practice only, not official BEA test items and not a validated prediction of the 2027 A&E.
- Item difficulty classification is provisional; field test is recommended.
- Some scientific inquiry and performance competencies are approximated via MCQs, which cannot replace performance assessments.
- App must be served via HTTPS for service-worker offline use; a file:// standalone HTML copy does not install as a PWA.
- When revising content, increment the cache version in BOTH `sw.js` and `index.html` to force a new offline bundle.
- For GitHub Pages hosting within one account, different repositories have different path scopes; each reviewer uses its own IDs, storage keys, and cache prefix.

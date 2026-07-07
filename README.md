# pan-yu-zurich.github.io

Personal academic website of Yu Pan.

## How this site deploys

- **The live site is built from the `main` branch** (plain static files, no build step). Push to `main` and GitHub Pages redeploys automatically, usually within a minute.
- **Do not touch or deploy from `gh-pages`.** That branch holds a retired April-2026 Hugo version of the site together with its own Actions deploy workflow; deploying it overwrites the live site with the old design (this happened on 2026-07-06).
- If a push does not seem to go live, check that a "pages build and deployment" run exists for your commit; pushes that land while another build is queued are sometimes skipped. Push an empty commit to retrigger.

## Editing content

Everything lives in `index.html`:

- **About / bio**: search for `renderHome`
- **News banner / upcoming talks**: search for `Latest Publication` or `Upcoming Conferences`
- **Publications**: search for `const publications`
- **Working papers**: search for `const workingPapers`
- **Work in progress**: search for `const inProgress`
- **Coauthor links**: search for `COAUTHOR_URLS`
- **Teaching**: search for `const ta`

## Papers policy (do not "fix" these)

- Working-paper PDFs live under `/papers/` and are linked **from the CV only**. The site deliberately does not link them, and `robots.txt` blocks search engines from that folder (one submission is under double-blind review).
- The paper under review at AMD is listed under a deliberately vague placeholder title ("Chinese Football"). Keep it that way until the review concludes.
- Solo-authored working papers (including the Job Market Paper) stay off the site until they reach Revise & Resubmit.
- The CV PDF is intentionally not hosted on the site.

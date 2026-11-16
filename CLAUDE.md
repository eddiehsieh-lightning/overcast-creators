# overcast-creators

Static site served by GitHub Pages from the `main` branch root, on the custom domain overcastcreators.com. There is no build step: what is committed is what is served.

## Layout

- `index.html` — the homepage. A single large self-contained file; do not read it whole.
- `<page-name>/index.html` — every other page, one folder each, served at `https://overcastcreators.com/<page-name>/`.
- `CNAME` — the custom domain. Do not edit or delete it; removing it takes the whole site off the domain.
- `.nojekyll` — tells GitHub Pages to serve files as they are. Keep it.

## Adding a page

1. Pick the folder name: lowercase, hyphens, brand prefix first, campaign ID last when there is one (`lop-fresh-glow-83518`, `drg-red-brief`). Check the name is not already taken here.
2. Write the page to `<page-name>/index.html`.
3. Keep the page self-contained, or reference its files with relative paths. A leading-slash path (`/style.css`) points at the homepage's root and breaks.
4. Do not add a `CNAME` file inside the folder, do not create a new repo, and do not ask for a DNS record. None are needed.
5. Tell the user the final link: `https://overcastcreators.com/<page-name>/`.

## Publishing

- A commit on `main` is live in about a minute. Confirm with the user before pushing to `main`; these pages go to creators.
- Never rename or delete a folder whose link may already have been sent. Edit in place instead.
- Keep each file under 25 MB so it can also be replaced through GitHub's web upload.

## Older pages

About 30 earlier pages live in separate repos under the same GitHub account, each on its own subdomain (`<name>.overcastcreators.com`). Leave them where they are unless the user asks to move one. Moving one changes its link, so the old subdomain repo must stay up or redirect.

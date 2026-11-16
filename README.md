# overcast-creators

The site at **overcastcreators.com**. The homepage is `index.html` at the top level. Every other page is a folder.

## Add a new page

1. Make a folder named for the page, lowercase with hyphens, for example `lop-fresh-glow-83518`.
2. Put the page inside it as `index.html`.
3. Commit to `main`.

About a minute later the page is live at `https://overcastcreators.com/lop-fresh-glow-83518/`.

There is no DNS step, no new repo and no CNAME file. The folder name is the link.

### Without any tools

On github.com, open this repo, choose **Add file → Upload files**, and drag the whole folder in (the folder, not just the file inside it). Commit the change.

### With Claude

Open this repo in Claude and say what you want, for example "add this brief as `lop-fresh-glow-83518`" or "change the commission line on `drg-red-brief`". Claude follows the rules in `CLAUDE.md`.

## Edit or remove a page

- **Edit:** replace the `index.html` in that page's folder and commit.
- **Remove:** delete the folder and commit. The link stops working, so only do this once nobody needs it.

## Rules

- One folder per page, and the file inside is always called `index.html`.
- Folder names are lowercase letters, numbers and hyphens only. No spaces.
- A folder name is permanent once the link has been sent out. To change a page, edit it in place.
- Pages should be self-contained (styles and images inside the one file) or use relative paths (`style.css`, not `/style.css`).
- Leave `CNAME`, `.nojekyll` and the top-level `index.html` alone unless you mean to change the domain or the homepage.

## Older pages

Pages published before this setup live in their own repos on their own subdomains (for example `drg-red-brief.overcastcreators.com`). Those links still work and are edited in their own repos. New pages go here.

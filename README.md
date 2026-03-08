# AI Web Drop

This repository is now set up as a drop-zone for HTML files.

## How it works

- `index.html` loads your repository tree from the GitHub API.
- It automatically finds every `.html` file in the repo.
- It excludes `index.html` itself.
- It renders clickable links to the remaining files.

## Use it

1. Add any new `.html` file anywhere in this repository.
2. Commit and push to GitHub.
3. Open your GitHub Pages site and the file appears automatically.

## GitHub Pages notes

- This is designed for GitHub Pages hostnames (`*.github.io`).
- It uses unauthenticated GitHub API requests, which are rate-limited.
- The repository must be public for the client-side API requests to work without a token.

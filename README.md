# AI Web Drop

A single-page drop-zone that lists every HTML file in this repo as browsable cards, served from GitHub Pages.

## How it works

- `index.html` loads the repository tree from the GitHub API
- It scans for every `.html` file in the repo (excluding `index.html`)
- Card titles and descriptions are pulled from `manifest.json`
- Cards link to the full HTML report, opening in a new tab

## Adding a new file

1. Add any `.html` file anywhere in the repository
2. Add an entry to `manifest.json` with a description
3. Commit and push — the card appears on the next page load

### manifest.json format

```json
{
  "My Report.html": "A brief description of what this report contains."
}
```

## GitHub Pages notes

- This is designed for GitHub Pages hostnames (`*.github.io`)
- It uses unauthenticated GitHub API requests, which are rate-limited
- The repository must be public for the client-side API requests to work without a token

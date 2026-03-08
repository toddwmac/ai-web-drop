# AI Web Drop

A polished drop-zone for HTML files on GitHub Pages.

## How it works

- `index.html` loads your repository tree from the GitHub API
- It automatically finds every `.html` file in the repo
- It excludes `index.html` itself
- It renders elegant cards with titles and descriptions
- Files open in new tabs

## Adding descriptions

Edit `manifest.json` to add descriptions for your files:

```json
{
  "My File.html": "A brief description of what this file contains."
}
```

The filename in the manifest must match the exact file path in your repository.

## Use it

1. Add any new `.html` file anywhere in this repository
2. Update `manifest.json` with a description for the file (optional)
3. Commit and push to GitHub
4. Open your GitHub Pages site and the file appears automatically

## GitHub Pages notes

- This is designed for GitHub Pages hostnames (`*.github.io`)
- It uses unauthenticated GitHub API requests, which are rate-limited
- The repository must be public for the client-side API requests to work without a token

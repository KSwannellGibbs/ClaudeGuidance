# Claude Guidance Hub — Enate

Source files for the live site at **http://enate-claude-guidance.netlify.app**

## What's in here

| File | Page |
|---|---|
| `index.html` | Hub landing page |
| `how-and-when-to-use-claude.html` | How & When to Use Claude (interactive tool) |
| `building-blocks-at-a-glance.html` | Claude's Building Blocks |
| `claude-cowork-tips-and-tricks.html` | How to Use Claude Cowork |
| `building-an-agent-with-claude-code.html` | Building an Agent with Claude Code |
| `token-usage-chat.html` | Getting More Out of Every Claude Message |
| `token-usage-cowork-code.html` | Getting More Out of Every Cowork & Code Session |
| `feedback.html` | Feedback form (Netlify Forms) |

All pages are self-contained static HTML — no build step, no dependencies. The Enate logo is embedded inline as base64 in each file.

## Setting this up in GitHub

1. Create a new repo in the Enate GitHub org (e.g. `claude-guidance-hub`)
2. Push these files to the repo root:
   ```
   git init
   git add .
   git commit -m "Initial commit: Claude Guidance Hub"
   git branch -M main
   git remote add origin <your-repo-url>
   git push -u origin main
   ```

## Linking Netlify to the repo

The site currently deploys via direct file upload (not from Git). To switch to Git-based deploys:

1. In the Netlify dashboard: **Site settings → Build & deploy → Link repository**
2. Choose the GitHub repo you just created
3. Build settings: leave the build command blank and set the publish directory to `/` (root) — these are static files, nothing to build
4. Once linked, every push to `main` will auto-deploy

Site ID: `3877fc9f-ce66-48df-ad9b-9568b798410b`
Netlify project: `enate-claude-guidance`

## Notes

- Notion page (parent guidance doc) links out to each page above — if you rename any file, update those links too: https://app.notion.com/p/3a696e85411c81c4bf06c9836031f9f3
- Feedback form submissions currently land in Netlify's Forms dashboard. An email notification to katie.gibbs@enate.net still needs to be set up manually in Site settings → Forms → Form notifications.

# Appeal Studio — Direct Mail Intelligence

A single-file browser app that generates complete, campaign-ready direct mail appeal briefs for nonprofits using the Claude API.

## What it does

Paste in an organization name, mission, and audience — Appeal Studio produces a structured 13-section appeal brief covering concept, copy strategy, package format, ask ladder, imagery, and more. A built-in refine flow lets you iterate on any section without regenerating the whole brief.

## How to use

1. Open `appeal-studio.html` in any modern browser (no build step, no server).
2. Enter your **Anthropic API key** in the key field (stored only in your browser session — never sent anywhere except the Anthropic API).
3. Fill in the required fields: org name, mission, audience.
4. Optionally expand the customization panel to set tone, mail date, colors, add-in type, and ask ladder amounts.
5. Click **Generate** and the brief appears inline.
6. Use the **Refine** tab to make targeted edits to specific sections.

## Requirements

- A valid [Anthropic API key](https://console.anthropic.com/)
- A modern browser (Chrome, Firefox, Safari, Edge)
- No Node, no npm, no build tools

## File structure

```
appeal-studio.html   # The entire app — HTML + CSS + React + app logic
```

## Development notes

- The app is intentionally a single HTML file for maximum portability — drop it anywhere, open it, it works.
- React 18 and Babel are loaded from CDN so no build step is needed.
- The full company-projects reference zip is excluded from version control (see `.gitignore`). It lives locally and is used only as a reference when improving the studio.
- To improve the app, edit `appeal-studio.html` directly. There is no compilation step.

## Contributing / iterating

When making improvements, keep the single-file constraint. If the file grows unwieldy, the right move is to extract CSS and JS into sibling files (`appeal-studio.css`, `appeal-studio.js`) — but only when needed.

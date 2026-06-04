# shiplog

Track AI-assisted requests, deliverables, status, and handoffs in one local dashboard.

![shiplog dashboard](shiplog-dashboard-preview.png)

## Who it is for

shiplog is for builders who work across many AI assistant sessions and need a simple way to see what was requested, what shipped, what is still open, and where the output landed.

It is part of grAIce Tech's work on operational clarity, agentic workflows, and practical systems for regulated work.

## Problem it solves

AI-assisted work often scatters across chats, local folders, repos, docs, and screenshots. Within a few days, it becomes hard to reconstruct what happened or decide what needs follow-up.

shiplog gives you a single-file dashboard for that record. No server, database, account, build step, npm package, or framework.

## Quickstart

```bash
curl -O https://raw.githubusercontent.com/grAIcetech/shiplog/main/shiplog.html
open shiplog.html
```

## Example output

The dashboard includes:

- Status counts and progress summary
- Search across requests, categories, channels, notes, and artifacts
- Filters for status and category
- Editable notes saved to `localStorage`
- Markdown export
- A responsive dark-mode table

## How it works

Open `shiplog.html` in any browser. To customize the data, edit the `DATA` array in the file:

```javascript
const DATA = [
  {
    id: 1,
    request: "Your request",
    category: "Category",
    channel: "Code",
    status: "Delivered",
    date: "2026-05-01",
    artifact: "path/or/url",
    notes: ""
  }
];
```

Categories generate filter buttons automatically. Status values drive the summary cards and table badges.

## Status / roadmap

Status: usable single-file dashboard.

Planned cleanup:

- Keep the file dependency-free.
- Improve starter data and examples.
- Add clearer guidance for maintaining a team or project-level shiplog.

## License

MIT. Built by [grAIce Tech](https://github.com/grAIcetech).

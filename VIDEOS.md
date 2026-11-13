# Managing videos

Videos on the page come from `videos.json`. To add one, edit that file on GitHub
(pencil icon), add an entry, and commit. Cloudflare redeploys automatically if the
Worker is connected to this repo.

```json
[
  { "title": "Mantra song", "url": "https://youtu.be/XXXXXXXXXXX", "show": true },
  { "title": "Site walkthrough", "url": "https://www.youtube.com/watch?v=YYYYYYYYYYY" }
]
```

- Order in the file = order on the page.
- `"show": false` hides a video without deleting it.
- Any YouTube link format works (youtu.be, watch?v=, shorts, embed).
- Keep commas between entries; no comma after the last one.

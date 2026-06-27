# Voltage — PhD vacancies in Electrical Engineering (Europe)

A static, manually-curated job board. Hosted free on GitHub Pages. No backend, no database.

## How to add a position
1. Open `positions.json`.
2. Copy one existing block and paste it inside the `[ ... ]`, separated by a comma.
3. Edit the fields. Only `link` and `title` are strictly required; the rest improve filtering/display.
4. Commit. The live site updates within ~1 minute.

```json
{
  "title": "PhD in ...",
  "institution": "University name",
  "country": "Germany",
  "city": "Munich",
  "subfield": "Power Electronics",
  "deadline": "2026-09-30",
  "funding": "Fully funded",
  "link": "https://the-original-posting-url",
  "added": "2026-06-26"
}
```

- `deadline` / `added`: use `YYYY-MM-DD`. A deadline within 14 days shows red.
- Country and subfield auto-populate the filter dropdowns — keep spelling consistent.
- To remove a position, delete its block.

## Deploy on GitHub Pages
1. Create a repo, e.g. `voltage` (or `<username>.github.io` for a root URL).
2. Upload `index.html` and `positions.json`.
3. Repo **Settings → Pages → Source: Deploy from branch → main / root**.
4. Your site goes live at `https://<username>.github.io/voltage/`.

That's it. Adding a job = editing one JSON file.

# How to Update Your Site

All content lives in `content.json`. Edit it, save, push. Site updates in ~30 seconds.

```bash
git add content.json
git commit -m "what you changed"
git push
```

---

## Socials
Only add a URL when you have the real link. Entries with `"#"` are hidden automatically.

```json
{ "label": "GitHub",       "url": "https://github.com/YOUR_USERNAME" }
{ "label": "YouTube",      "url": "https://youtube.com/@YOUR_CHANNEL" }
{ "label": "ResearchGate", "url": "https://researchgate.net/profile/YOUR_PROFILE" }
{ "label": "X / Twitter",  "url": "https://x.com/YOUR_HANDLE" }
```

---

## Add a project
```json
{
  "title": "Your title",
  "year": "2026",
  "status": "in progress",
  "description": "Write this yourself.",
  "description2": "",
  "tags": ["tag1", "tag2"],
  "links": [
    { "label": "GitHub", "url": "https://github.com/you/repo" }
  ]
}
```
Leave `"status": ""` if not needed. Leave `"links": []` if nothing to link yet.

---

## Add a paper
```json
{
  "status": "Published",
  "title": "Full title as published",
  "authors": "Sachin Raj",
  "abstract": "Your abstract here.",
  "links": [
    { "label": "Journal", "url": "https://..." },
    { "label": "PDF",     "url": "https://..." }
  ]
}
```
Status options: `"Published"` · `"In review"` · `"Forthcoming"`

---

## Add a tool
```json
{
  "name": "tool-name",
  "version": "v1.0.0",
  "type": "free",
  "description": "What it does.",
  "tags": ["tag1", "tag2"],
  "links": [
    { "label": "GitHub", "url": "https://github.com/you/tool" },
    { "label": "PyPI",   "url": "https://pypi.org/project/tool/" }
  ]
}
```
Use `"type": "commercial"` for paid tools.

---

## Add a blog post
Add at the **top** of the `"posts"` array (newest first):
```json
{
  "date": "August 2026",
  "title": "Your post title",
  "excerpt": "One paragraph in your own words."
}
```

---

## Update your intro
Find `"intro"` — it's an array of strings, one per paragraph. Edit the text directly.

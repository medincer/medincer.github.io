---
title: Wiki Links
feed: show
date: 2024-01-15
---

Wiki links let you connect your notes using double brackets, like `[[Note Title]]`. This works exactly like linking notes in Obsidian.

## How to Use

Simply type `[[Note Title]]` in your note. If a note with that title exists, it becomes a clickable link. If not, you'll see a placeholder indicating the note doesn't exist yet.

You can also link to external websites: `[[Google::https://google.com]]`.

## Examples

```markdown
This note connects to [[Getting Started]] and [[Markdown Guide]].

For more information, check out [[Jekyll::https://jekyllrb.com]].
```

## Automatic Backlinks

When you create a wiki link to another note, that note automatically shows a "Backlinks" section. For example, if you visit [[Getting Started]], you'll see this note listed there because we linked to it.


## Troubleshooting

If a wiki link appears broken:
1. Check the exact spelling of the note title
2. Make sure the note exists in the `_notes` folder
3. Verify the note has `feed: "show"` in its front matter

---

*Wiki links transform your notes from isolated documents into a connected knowledge base.* 
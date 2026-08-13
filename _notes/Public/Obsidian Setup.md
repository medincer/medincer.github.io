---
title: Obsidian Setup
feed: show
date: 2024-01-15
---

Here's how to set up Jekyll Garden to work seamlessly with Obsidian.

## Use `_notes` as Your Vault

The simplest approach is to use the `_notes` folder as your Obsidian vault:

1. **Open Obsidian**
2. **Create a new vault** or open existing vault
3. **Set the vault location** to the `_notes` folder in your Jekyll Garden project

This way, all your notes are automatically part of your website.

## Front Matter Requirements

All notes must use the proper front matter format:

```yaml
---
title: "Your Note Title"
date: 2024-01-15
feed: "show"
---
```

The `feed: "show"` setting makes the note appear on your website. Use `feed: "hide"` for private notes.

## Git Ignore Setup

Add these folders to your `.gitignore` file:

```gitignore
# Obsidian settings
.obsidian/
.trash/

# Jekyll build files
_site/
.sass-cache/
.jekyll-cache/
```

## Private Notes

To keep some notes private (not published on your website):

1. **Create a folder** inside `_notes` (e.g., `_notes/Private/`)
2. **Add the folder to `.gitignore`**:
   ```gitignore
   _notes/Private/
   ```
3. **Set `feed: "hide"`** in the note's front matter

This way, private notes stay in your Obsidian vault but won't be synced to Git or built as pages in Jekyll.

## Workflow

1. **Write notes** in Obsidian using the `_notes` folder
2. **Use [[Wiki Links]]** to connect your notes
3. **Add proper front matter** to each note
4. **Commit and push** to publish changes
5. **Your website updates** automatically

## Tips

- **Keep Obsidian and Jekyll in sync**: The `_notes` folder is your single source of truth
- **Use descriptive titles**: They become your URLs and link targets
- **Test locally**: Run `bundle exec jekyll serve` to preview changes
- **Backup regularly**: Your notes are valuable - keep them safe

## External Resources

- [Obsidian Documentation](https://obsidian.md/help)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages](https://pages.github.com/)

---

*This setup gives you the best of both worlds: powerful note-taking in Obsidian and beautiful publishing with Jekyll Garden.* 
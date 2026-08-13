# Jekyll Garden
![screenshot](https://github.com/user-attachments/assets/f5752b1a-eb11-4385-a2ad-09f0e698ad30)
A simple Jekyll theme that turns your Obsidian notes into a beautiful website. Perfect for sharing your thoughts and knowledge online. If you use Obsidian for note-taking, this theme makes it easy to publish your markdown files as a connected website with wiki-style links and full-text search.


### What it does

Jekyll Garden connects your notes together with simple `[[note title]]` links, just like in Obsidian. You can find any note quickly with the built-in search that works as you type. The design focuses on your content with a clean, minimal look that works great on phones, tablets, and computers. Choose between dark and light themes, and when you want to write traditional blog posts, you can do that too. The theme also supports mathematical expressions if you need to write equations.

## Getting Started

Getting started is straightforward. First, download this theme to your computer. Then edit the settings in the `_config.yml` file with your website information. Add your notes to the `_notes` folder, and finally deploy to GitHub Pages, Netlify, or any web hosting service.

## Basic Setup

Edit `_config.yml` with your information:

```yaml
title: "My Website"
heading: "Your Name"
description: "A brief description of your site"
url: "https://yoursite.com"
```

### Deployment Options

You can deploy your site to a subdomain (like `notes.yoursite.com`) or a subdirectory (like `yoursite.com/notes`):

**For subdomains:**
```yaml
url: "https://notes.yoursite.com"
baseurl: ""
```

**For subdirectories:**
```yaml
url: "https://yoursite.com"
baseurl: "/notes"
```

See `SUBDOMAIN_SETUP.md` for more details.

## Writing Notes

### Creating a Note

Each note is just a markdown file with a title. You write your content in markdown format, just like you would in Obsidian or any other markdown editor.

```yaml
---
title: "My First Note"
date: 2025-01-15
---
```

## Features

### Linking Notes Together
Connect your notes by using `[[note title]]` to link to other notes. This creates the same kind of connections you're used to in Obsidian, but now they work on your website too.


### Simple Linking
The linking system works just like Obsidian. Write `[[note title]]` and the links are created automatically. When you hover over a link, you'll see a preview of the connected note.

### Search
Finding content is easy with the built-in search. It searches through all your notes instantly as you type, looking at both titles and content to help you find exactly what you need.

### Backlinks
See which notes link to the current one you're reading. This helps you discover related content and explore the connections between your ideas, just like the backlinks feature in Obsidian.

### Math
If you need to write mathematical expressions, the theme supports it. Use `$x = y$` for inline math and `$$\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}$$` for complex equations.

## How to Publishing Your Site

### GitHub Pages (Free)
GitHub Pages is the easiest way to get started. Upload your files to GitHub, enable GitHub Pages in the repository settings, and your site goes live automatically.

### Netlify (Free)
Netlify is another great option. Connect your GitHub repository to Netlify, and it will build and host your site. Every time you update your files, your site updates automatically.

### Local Testing
Test your site locally before publishing. Run `bundle install` to install dependencies, then `bundle exec jekyll serve` to start a local server and see your site in action.

### Customization
Change the look of your site by editing the `assets/css/style.css` file. You can modify colors, fonts, and other visual elements to match your preferences. If you want to customize the layout, you can modify files in the `_layouts/` folder. Add your own CSS and JavaScript as needed, but remember to keep it simple.

## Contributing
Found a bug or have an idea for improvement? Contributions are welcome. Fork the repository, make your changes, and submit a pull request.

## License

MIT License - use it freely for any project.

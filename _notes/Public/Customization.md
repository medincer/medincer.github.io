---
title: Customization
feed: show
date: 2024-01-15
---

You can customize your Jekyll Garden site by editing a few key files.

## Basic Settings

Edit `_config.yml` to change your site information:

```yaml
title: "My Digital Garden"
heading: "Your Name"
description: "A brief description of your site"
url: "https://yoursite.com"
```

## Menu Items

Add or change navigation menu items:

```yaml
menu:
  - title: "Notes"
    url: "/notes"
  - title: "About"
    url: "/about"
  - title: "Blog"
    url: "/blog"
```

## Theme Preferences

Control which features are enabled:

```yaml
preferences:
  homepage:
    enabled: true      # Show custom homepage
  search:
    enabled: true      # Enable search
  backlinks:
    enabled: true      # Show backlinks
```

## Colors and Fonts

Change the look by editing `assets/css/style.css`:

```css
:root {
  --primary-color: #007acc;
  --text-color: #333;
  --background-color: #fff;
  --font-family: -apple-system, BlinkMacSystemFont, sans-serif;
}
```

## Dark Mode

The theme includes automatic dark mode support. Users can toggle between light and dark themes, and their preference is saved.

## Custom Fonts

Add custom fonts by importing them in the CSS:

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap');

:root {
  --font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
}
```

## Layout Changes

For advanced customization, you can modify files in the `_layouts/` folder. But remember to keep it simple - focus on content over complex styling.

## Tips

- Start with basic settings in `_config.yml`
- Test changes locally before deploying
- Keep customization minimal for better performance
- Use the [[Deployment]] guide when you're ready to publish

---

*Customization should enhance your content, not distract from it.* 
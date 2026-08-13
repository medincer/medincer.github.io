---
title: Deployment
feed: show
date: 2024-01-15
---

Once you've set up your Jekyll Garden site, here's how to publish it online.

## GitHub Pages (Free)

GitHub Pages is the easiest way to get started:

1. **Upload your files** to a GitHub repository
2. **Enable GitHub Pages** in repository settings
3. **Set source** to "Deploy from a branch"
4. **Choose your main branch** (usually `main` or `master`)

Your site will be available at `https://yourusername.github.io/repository-name`

## Netlify (Free)

Netlify offers automatic deployments:

1. **Connect your GitHub repository** to Netlify
2. **Set build command**: `bundle exec jekyll build`
3. **Set publish directory**: `_site`
4. **Deploy automatically** when you push changes

## Vercel (Free)

Vercel is another great option:

1. **Import your repository** to Vercel
2. **Framework preset**: Jekyll
3. **Deploy automatically** on every push

## Local Testing

Test your site before deploying:

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000` to see your site.

## Custom Domain

Add your own domain in `_config.yml`:

```yaml
url: "https://yourdomain.com"
```

Then configure your domain with your hosting provider.

## Tips

- **Test locally first**: Make sure everything works before deploying
- **Check your links**: Ensure all [[Wiki Links]] work correctly
- **Optimize images**: Compress images for faster loading
- **Use HTTPS**: Most hosting providers offer this automatically

## Troubleshooting

**Site not updating?**
- Check that your changes are pushed to the repository
- Verify the build completed successfully
- Clear your browser cache

**Broken links?**
- Ensure all note titles match exactly
- Check that notes have `feed: "show"` in front matter
- Rebuild your site after adding new notes

---

*Your digital garden is ready to share with the world!* 
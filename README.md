# Will Button's Blog

Personal blog covering crypto technology for the over-40 crowd, fitness, and outdoors.

## Development

```bash
# Install Hugo (macOS)
brew install hugo

# Run development server
hugo server --buildDrafts

# Build for production
hugo --minify
```

## Deployment

This site is configured for **GitHub Pages** deployment:

### Setup Steps
1. **Create GitHub repository** for your site
2. **Push your code** to the `main` branch
3. **Enable GitHub Pages** in repository Settings > Pages
4. **Set source** to "GitHub Actions"
5. **Point your domain** in Route 53 to GitHub Pages

### Custom Domain (Route 53)
1. In your GitHub repo: Settings > Pages > Custom domain: `willbutton.com`
2. In Route 53, create these records:
   ```
   Type: A
   Name: @ (or blank)
   Value: 185.199.108.153
          185.199.109.153
          185.199.110.153
          185.199.111.153
   
   Type: CNAME  
   Name: www
   Value: willbutton.github.io
   ```

The GitHub Action will automatically build and deploy on every push to `main`.

## Writing Posts

Create new posts with:

```bash
hugo new posts/my-new-post.md
```

Posts should include categories (crypto, fitness, outdoors) and relevant tags.

## Theme

Once you select a theme, add it as a git submodule:

```bash
git submodule add https://github.com/theme-author/theme-name themes/theme-name
```

Then update `hugo.toml` to set `theme = "theme-name"`.
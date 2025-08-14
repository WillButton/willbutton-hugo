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

This site is configured for **Cloudflare Pages** deployment:

- **Build command**: `hugo --minify`
- **Build output directory**: `public`
- **Node.js version**: Latest

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
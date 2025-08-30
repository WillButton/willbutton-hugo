# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is Will Button's personal brand blog built with Hugo using the PaperMod theme. The site positions Will as "The 30-Year Tech Veteran Learning DeFi" and focuses on three main content pillars. It's deployed to GitHub Pages with automatic builds via GitHub Actions.

## Brand Positioning

**Core Identity:** "From Flight Decks to DeFi" - Navy Nuclear Engineer turned Engineering Manager at katana, learning DeFi in public after 30 years of tech evolution.

**Target Audience:** 
- Primary: Technical and non-technical people wanting to understand/succeed in DeFi
- Secondary: Experienced tech professionals considering Web3 transitions  
- Tertiary: High performers seeking sustainable excellence across life domains

**Value Proposition:** Learn DeFi from someone who's survived and thrived through 30 years of tech evolution while maintaining peak physical and mental performance.

## Development Commands

```bash
# Install Hugo (if not already installed)
brew install hugo

# Start development server with draft posts visible
hugo server --buildDrafts

# Start development server (published posts only)
hugo server

# Build for production
hugo --minify

# Create new post
hugo new posts/my-new-post.md
```

## Content Structure

**Three Main Categories:**
- `defi` - DeFi education, protocol analysis, learning-in-public content (40% of content)
- `performance` - Four Spinning Plates philosophy, sustainable high performance (25% of content)  
- `career` - 30-year tech career wisdom, adaptation strategies, leadership lessons (25% of content)

**Content Calendar:**
- Monday: DeFi Learning (protocol analysis, tokenomics breakdowns)
- Wednesday: Four Spinning Plates (fitness, mental health, life philosophy)
- Friday: Tech Career Wisdom (leadership lessons, career evolution)
- Weekend: Personal updates and behind-the-scenes content

**Post Format Requirements:**
- `categories: ["defi"|"performance"|"career"]`
- `tags: [relevant tags including "learning-in-public" for DeFi content]`
- `draft: false` when ready to publish
- Optional `cover` section with image, alt text, and caption
- Include disclaimers for financial content
- Use engineering/systems thinking analogies

## Writing Style Guidelines

- **Tone**: Direct, authentic, no hype - "engineering discipline applied"
- **Audience**: Experienced professionals over 40 who want actionable insights
- **Approach**: Learning in public, sharing failures and lessons learned
- **Perspective**: 30 years of tech experience applied to new domains
- **Format**: Use personal examples, systematic frameworks, proven methodologies

## The Four Spinning Plates Framework

Core philosophy for sustainable high performance:
1. **Physical Health** - 100K ultra finisher while working full-time
2. **Mental Health** - Stress management from high-pressure environments
3. **Family Relationships** - Maintaining connections through career growth
4. **Financial Success** - Building wealth through calculated risks

## Site Configuration

- **Base URL**: https://willbutton.com
- **Theme**: PaperMod (installed as git submodule in `themes/PaperMod/`)
- **Navigation**: DeFi Journey, Four Plates, Tech Career, About
- **Description**: "30-year tech veteran learning DeFi in public. Making complex protocols accessible while maintaining peak performance across life's four spinning plates."

## Deployment

GitHub Pages with automated deployment via `.github/workflows/hugo.yml`. Pushes to `main` trigger builds using Hugo 0.148.2 with extended features and Dart Sass.

## Content Creation Notes

- Store images in `static/images/` and reference as `/images/filename.ext`
- Use systematic risk assessment frameworks for DeFi content
- Apply military/engineering analogies to explain complex concepts
- Share personal learning journey and mistakes transparently
- Focus on long-term sustainability over short-term gains
- Bridge traditional tech knowledge with Web3 concepts
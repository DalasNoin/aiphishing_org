# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Academic research website for the paper "Evaluating Large Language Models' Capability to Launch Fully Automated Spear Phishing Campaigns" (arXiv:2412.00586). Hosted at aiphishing.org via GitHub Pages.

## Development Commands

```bash
# Install dependencies
bundle install

# Run local development server
bundle exec jekyll serve
```

The site will be available at http://localhost:4000

## Architecture

**Static Site Generator**: Jekyll with GitHub Pages remote theme (pages-themes/cayman)

**Key Files**:
- `_config.yml` - Site configuration, navigation links, and SASS settings
- `_layouts/default.html` - Base layout template with header navigation
- `index.html` - Main research summary page with results and figures
- `demo.html` - Interactive comparison of AI-generated phishing emails from different models
- `leaderboard.html` - Model performance comparison table (currently commented out in navigation)
- `signup.html` - Google Forms signup redirect page

**Styling**:
- `assets/css/style.scss` - Main SCSS file importing the theme plus custom styles
- `assets/css/custom.css` - Additional CSS overrides for email comparison layout

**Content**: Pages use Jekyll front matter (`layout: default`) and inline `<style>` blocks for page-specific styles.

## Navigation

Navigation is configured in `_config.yml` under `navigation:`. The leaderboard page exists but is currently commented out from the nav.

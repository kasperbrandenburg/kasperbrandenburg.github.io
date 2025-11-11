# Copilot Instructions for kasperbrandenburg.github.io

This repository is a knowledge base and security research website hosted via GitHub Pages, using the Just the Docs Jekyll theme. Follow these guidelines for effective AI agent contributions:

## Project Overview
- **Type:** Knowledge base website (Jekyll, GitHub Pages)
- **Theme:** Just the Docs (`remote_theme: just-the-docs/just-the-docs@v0.10.1`)
- **Custom Domain:** Set via `CNAME` to `www.kasperbrandenburg.dk`
- **Purpose:** Security research, vulnerability disclosures, and technical documentation

## Site Structure
```
├── index.html          # Homepage (converted to markdown-style)
├── about.md           # About page with professional background
├── contact.md         # Contact information and disclosure guidelines
├── advisories/        # Security advisories directory
│   ├── index.md       # Advisories overview page
│   └── *.md          # Individual security advisories
├── _config.yml       # Jekyll configuration with Just the Docs settings
├── Gemfile           # Ruby dependencies for local development
└── CNAME             # Custom domain configuration
```

## Key Patterns & Conventions

### Navigation Structure
- **Left sidebar navigation** automatically generated from page frontmatter
- **nav_order**: Controls menu position (lower numbers appear first)
- **parent/has_children**: Creates hierarchical navigation structure
- **title**: Appears in navigation menu and page header

### Page Creation Guidelines
1. **Security Advisories**: Create in `/advisories/` directory with:
   - `parent: Security Advisories` in frontmatter
   - Structured format: Description, Technical Details, Impact, Mitigation
   - Both English and Danish content where applicable
   - CVE references and external links

2. **Regular Pages**: Create in root directory with:
   - Descriptive `title` and `description` frontmatter
   - Appropriate `nav_order` for menu positioning
   - Consistent markdown structure

### Content Language
- **Primary**: English for technical content and navigation
- **Secondary**: Danish for specific advisories or local content
- **Bilingual approach**: Include both languages for security advisories when relevant

### Theme Features
- **Built-in search**: Automatically indexes all content
- **Responsive design**: Mobile-friendly left sidebar navigation
- **Color scheme**: Auto light/dark mode based on system preference
- **SEO optimization**: Built-in meta tags and structured data

## File Management
- **Markdown preferred**: Use `.md` files for new content
- **Frontmatter required**: All pages need YAML frontmatter for proper navigation
- **Asset organization**: Place images and files in logical subdirectories
- **Clean URLs**: Jekyll automatically generates clean URLs from file structure

## Development Workflow
- **Local development**: Use `bundle exec jekyll serve` for testing
- **GitHub Pages deployment**: Automatic on push to main branch
- **Configuration changes**: Modify `_config.yml` for theme settings
- **Dependency management**: Update `Gemfile` for new Jekyll plugins

## Security Advisory Template
```yaml
---
layout: default
title: "Advisory Title"
parent: Security Advisories
nav_order: [number]
description: "Brief description for SEO"
---

# Advisory Title

## Technical Details
- CVE/Vulnerability information
- Affected systems
- Impact assessment

## Mitigation
- Recommended solutions
- Implementation steps

## References
- External links and resources
```

---
For questions about site structure, theme customization, or security content guidelines, refer to the Just the Docs documentation or repository owner.

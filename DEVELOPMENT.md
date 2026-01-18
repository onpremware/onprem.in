# onprem.in - Development Guide

A modern, minimalistic website for on-premise software solutions with a distinctive hacker-aesthetic design.

## Overview

Built with Astro 5, featuring:
- Clean, terminal-inspired design with green accent (#44d62c)
- Fully responsive navigation
- Blog with content collections (5 in-depth technical posts)
- Products showcase page
- Solutions page for different customer segments
- Optimized for performance and SEO

## Project Structure

```
/
├── public/              # Static assets
├── src/
│   ├── components/      # Reusable components
│   │   ├── Landing.astro
│   │   └── Navigation.astro
│   ├── content/         # Content collections
│   │   ├── blog/        # Blog posts (markdown)
│   │   └── config.ts    # Content schema
│   ├── layouts/
│   │   └── Layout.astro # Base layout
│   └── pages/
│       ├── index.astro       # Homepage
│       ├── products.astro    # Products page
│       ├── solutions.astro   # Solutions page
│       ├── blog/
│       │   ├── index.astro   # Blog listing
│       │   └── [slug].astro  # Blog post template
└── package.json
```

## Getting Started

### Install Dependencies
```bash
npm install
```

### Development Server
```bash
npm run dev
```
Visit http://localhost:4321

### Build for Production
```bash
npm run build
```

### Preview Production Build
```bash
npm run preview
```

## Content Management

### Adding Blog Posts

Create a new markdown file in `src/content/blog/`:

```markdown
---
title: "Your Post Title"
description: "Brief description of the post"
publishDate: 2026-02-01
category: "Security" # Security, Infrastructure, Self-Hosting, Enterprise, or Technical
tags: ["tag1", "tag2"]
author: "Author Name"
draft: false
---

# Your content here
```

### Content Categories

- **Security**: Security, compliance, data protection
- **Infrastructure**: Kubernetes, DevOps, systems
- **Self-Hosting**: Self-hosting guides and tips
- **Enterprise**: Enterprise case studies and strategies
- **Technical**: Deep technical guides

## Design System

### Colors

- **Background**: `#0a0a0f` (dark)
- **Primary Green**: `#44d62c`
- **Text Primary**: `#e4e4e7`
- **Text Secondary**: `#a1a1aa`
- **Text Muted**: `#71717a`

### Typography

- **Headings**: Space Grotesk (Google Fonts)
- **Code/Mono**: JetBrains Mono (Google Fonts)
- **Body**: Space Grotesk

### Key Design Elements

- Grid background overlay
- Animated green glow effects
- Floating particles on homepage
- Terminal-style breadcrumbs
- Monospace accents throughout
- Subtle animations on scroll

## Pages

### Homepage (/)
- Hero section with animated background
- Feature highlights
- Call-to-action

### Products (/products)
- 6 product cards with features
- Philosophy section
- Waitlist CTA

### Solutions (/solutions)
- Three customer segments: Enterprise, Startups, SMB
- Use cases grid
- Process timeline
- Consultation CTA

### Blog (/blog)
- Filterable post listing
- Category tags
- 5 in-depth technical articles

### Blog Posts (/blog/[slug])
- Full markdown support
- Code syntax highlighting
- Related posts
- Back navigation

## SEO & Meta

Each page has customizable:
- Title
- Description
- Open Graph tags

Defined in Layout.astro props.

## Performance

- Static site generation
- Optimized fonts with preconnect
- Minimal JavaScript (only for blog filters)
- CSS-only animations
- No external dependencies beyond Astro

## Deployment

The site is configured for static deployment. Compatible with:
- Vercel
- Netlify
- GitHub Pages
- Any static hosting

Build output is in `/dist`

---

Built with Astro 🚀

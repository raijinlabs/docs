# System Patterns: Raijin Labs Documentation

## Architecture Overview

Mintlify docs-as-code platform with Git-based workflow:

```
GitHub (raijinlabs/docs)
    |
    | Push to main branch
    v
Mintlify Dashboard
    |
    | Auto-build + deploy
    v
Public Documentation Site
    |
    | CDN-served static pages
    v
End Users (developers, partners)
```

## Content Architecture

### Navigation Structure (docs.json)

Two-tab layout:
- **Guides tab**: Getting started, Customization, Writing content, AI tools
- **API reference tab**: API documentation, Endpoint examples

### File Organization Pattern

```
c:\docs/
├── docs.json              # Central config (nav, theme, branding)
├── index.mdx              # Homepage
├── quickstart.mdx         # Getting started guide
├── development.mdx        # Local dev setup
├── ai-tools/              # AI tool integration guides
│   ├── cursor.mdx
│   ├── claude-code.mdx
│   └── windsurf.mdx
├── api-reference/          # API documentation
│   ├── introduction.mdx
│   ├── openapi.json        # OpenAPI spec (auto-generates endpoints)
│   └── endpoint/           # Endpoint examples
│       ├── get.mdx
│       ├── create.mdx
│       ├── delete.mdx
│       └── webhook.mdx
├── essentials/             # Content writing guides
│   ├── markdown.mdx
│   ├── code.mdx
│   ├── images.mdx
│   ├── navigation.mdx
│   ├── settings.mdx
│   └── reusable-snippets.mdx
├── snippets/               # Reusable MDX snippets
│   └── snippet-intro.mdx
├── images/                 # Static images
├── logo/                   # Brand logos (light/dark)
├── memory-bank/            # AI context files
├── .clinerules/            # Cline rules
└── docs/                   # Additional deep-dive docs
```

## Key Patterns

### 1. MDX Content Pattern
All content pages use MDX format with Mintlify components:

```mdx
---
title: "Page Title"
description: "Page description for SEO"
---

## Section

<Card title="Feature" icon="rocket" href="/link">
  Description of the feature.
</Card>
```

### 2. OpenAPI Auto-Generation
API reference pages are auto-generated from `api-reference/openapi.json`.
Mintlify reads the spec and creates interactive endpoint documentation.

### 3. Reusable Snippets
Common content blocks in `snippets/` directory, imported via MDX:

```mdx
<Snippet file="snippet-intro.mdx" />
```

### 4. Theme Configuration
All branding in `docs.json`:
- Colors (primary, light, dark)
- Logo (light/dark variants)
- Navigation structure
- Footer socials
- Navbar links

### 5. Git-Based Deployment
- Push to `main` branch triggers auto-deploy
- Mintlify GitHub app watches for changes
- No CI/CD pipeline needed (Mintlify handles build)

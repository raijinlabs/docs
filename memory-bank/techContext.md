# Tech Context: Raijin Labs Documentation

## Technology Stack

| Technology | Version | Purpose |
|-----------|---------|---------|
| Mintlify | Latest | Documentation platform |
| MDX | - | Content format (Markdown + JSX) |
| OpenAPI | 3.x | API spec format |
| Git/GitHub | - | Version control + deployment trigger |

## Development Setup

### Prerequisites
- Node.js (for Mintlify CLI)
- Git

### Commands

```bash
# Install Mintlify CLI globally
npm i -g mint

# Start local development server
cd c:\docs
mint dev
# Preview at http://localhost:3000

# Update Mintlify CLI
mint update
```

### Configuration

| File | Purpose |
|------|---------|
| `docs.json` | Central config: navigation, theme, branding, footer |
| `api-reference/openapi.json` | OpenAPI spec for auto-generated API docs |
| `favicon.svg` | Browser tab icon |
| `logo/light.svg` | Logo for light mode |
| `logo/dark.svg` | Logo for dark mode |

## Deployment

| Target | Platform | Trigger |
|--------|----------|---------|
| Production | Mintlify CDN | Push to `main` branch |
| Preview | Local | `mint dev` (localhost:3000) |

### Mintlify Dashboard
- GitHub app installed from [dashboard](https://dashboard.mintlify.com)
- Auto-deploys on push to default branch
- No manual build step required

## Content Format

### MDX Components Available
- `<Card>` - Feature cards with icons
- `<Columns>` - Multi-column layouts
- `<Tabs>` - Tabbed content
- `<Accordion>` - Collapsible sections
- `<Snippet>` - Reusable content blocks
- `<CodeGroup>` - Multi-language code blocks
- `<Warning>` / `<Note>` / `<Tip>` - Callout blocks

### Frontmatter
Every `.mdx` file starts with YAML frontmatter:
```yaml
---
title: "Page Title"
description: "SEO description"
icon: "icon-name"  # Optional Mintlify icon
---
```

## Repository Info

- **GitHub**: `raijinlabs/docs`
- **Origin**: `https://github.com/raijinlabs/docs.git`
- **Default Branch**: main
- **License**: See LICENSE file

## Related Repositories

| Repo | Relationship |
|------|-------------|
| `LucidMerged` | Main platform (docs reference its APIs) |
| `Lucid-L2` | AI backend (API docs generated from its OpenAPI spec) |
| `lucid-plateform-core` | Core services (TrustGate API docs) |
| `yaku-hub` | Additional services |

## Code Style for Documentation

- **File names**: `kebab-case.mdx`
- **Titles**: Title Case
- **Descriptions**: Sentence case
- **Code blocks**: Always specify language
- **Links**: Use relative paths within docs
- **Images**: Store in `images/` directory

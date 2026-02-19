# PROJECT MAP: Raijin Labs Documentation

## High-Level Architecture

```
Mintlify Docs Site (raijinlabs/docs)
├── docs.json          <- Central config (nav, theme, branding)
├── Content Pages      <- MDX files organized by topic
├── API Reference      <- Auto-generated from OpenAPI spec
└── Static Assets      <- Images, logos, favicon
```

## Module / Directory List

| Directory | Purpose | Key Files |
|-----------|---------|-----------|
| `/` (root) | Top-level pages + config | `docs.json`, `index.mdx`, `quickstart.mdx`, `development.mdx` |
| `ai-tools/` | AI tool integration guides | `cursor.mdx`, `claude-code.mdx`, `windsurf.mdx` |
| `api-reference/` | API documentation | `introduction.mdx`, `openapi.json` |
| `api-reference/endpoint/` | Endpoint examples | `get.mdx`, `create.mdx`, `delete.mdx`, `webhook.mdx` |
| `essentials/` | Content writing guides | `markdown.mdx`, `code.mdx`, `images.mdx`, `navigation.mdx`, `settings.mdx`, `reusable-snippets.mdx` |
| `snippets/` | Reusable MDX fragments | `snippet-intro.mdx` |
| `images/` | Static images | `hero-dark.png`, `hero-light.png`, `checks-passed.png` |
| `logo/` | Brand logos | `light.svg`, `dark.svg` |
| `memory-bank/` | AI context (Cline memory) | Core files (projectbrief, progress, etc.) |
| `.clinerules/` | Cline behavior rules | `00-context.md`, `01-memory-bank.md` |
| `docs/` | Deep-dive documentation | `PROJECT_MAP.md` |

## Key Flows

### Content Update Flow
1. Edit MDX file locally
2. Preview with `mint dev`
3. Push to `main` branch
4. Mintlify auto-deploys

### Adding a New Page
1. Create `.mdx` file in appropriate directory
2. Add frontmatter (title, description)
3. Add page path to `docs.json` navigation
4. Preview and deploy

### Adding API Endpoint
1. Update `api-reference/openapi.json` with new endpoint
2. Mintlify auto-generates the endpoint page
3. Optionally create custom MDX page in `api-reference/endpoint/`

## Where to Change Common Things

| Want to change... | Edit this file |
|-------------------|---------------|
| Site name/branding | `docs.json` |
| Navigation structure | `docs.json` > `navigation` |
| Homepage content | `index.mdx` |
| API endpoints | `api-reference/openapi.json` |
| Theme colors | `docs.json` > `colors` |
| Logo | Replace files in `logo/` |
| Add new guide page | Create `.mdx` + add to `docs.json` nav |
| Reusable content | Add to `snippets/` |
| Footer links | `docs.json` > `footer` |

## Glossary

| Term | Definition |
|------|-----------|
| MDX | Markdown + JSX - content format used by Mintlify |
| docs.json | Central configuration file for the documentation site |
| OpenAPI | Standard for API specification (auto-generates API docs) |
| Mintlify | Documentation platform (docs-as-code) |
| Snippet | Reusable MDX content block |

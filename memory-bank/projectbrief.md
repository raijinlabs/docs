# Project Brief: Raijin Labs Documentation (docs)

## Core Purpose
This is the **public-facing documentation site** for Raijin Labs products, built with [Mintlify](https://mintlify.com). It serves as the unified documentation hub covering:

1. **Lucid-L2 API Reference**  Unified AI endpoint for 100+ LLM models
2. **Platform Guides**  Getting started, quickstart, development setup
3. **AI Tools Integration**  Cursor, Claude Code, Windsurf integration guides
4. **API Endpoint Examples**  CRUD operations, webhooks

## Repository
- **GitHub**: aijinlabs/docs
- **URL**: https://github.com/raijinlabs/docs.git
- **Framework**: Mintlify (MDX-based documentation platform)

## Key Value Propositions

### For Developers
- Quick onboarding to Raijin Labs APIs and SDKs
- Interactive API reference with OpenAPI spec
- Copy-paste code examples in multiple languages
- AI tool integration guides (Cursor, Claude Code, Windsurf)

### For Partners & Enterprise
- Clear API documentation for integration
- Webhook setup guides
- Authentication and authorization docs

### For Internal Teams
- Single source of truth for all product documentation
- Version-controlled content (Git-based)
- Auto-deploy on push to default branch via Mintlify

## Success Criteria
1. Documentation covers all Raijin Labs products (Lucid-L2, LucidMerged, OpenClaw)
2. API reference is auto-generated from OpenAPI specs
3. < 2 minute time-to-first-API-call for new developers
4. 95%+ pages have code examples
5. Search works across all documentation

## Current Status (February 2026)

### Completed 
- Mintlify project scaffolded with starter kit
- Basic navigation structure (Guides + API Reference tabs)
- AI tools section (Cursor, Claude Code, Windsurf)
- API endpoint examples (GET, POST, DELETE, Webhook)
- OpenAPI spec integration
- Logo and branding assets

### In Progress 
- Customizing content from starter kit defaults to Raijin Labs products
- Lucid-L2 API documentation
- LucidMerged platform guides
- OpenClaw integration documentation

### Future Roadmap 
- SDK documentation (JavaScript, Python)
- Interactive API playground
- Changelog/release notes section
- Community guides and tutorials
- Multi-language support

## Target Audience

### Primary
- **Developers** integrating Lucid-L2 API
- **Platform Users** onboarding to LucidMerged
- **AI Engineers** using OpenClaw agents

### Secondary
- **Enterprise Partners** evaluating the platform
- **Open Source Contributors** extending the ecosystem
- **Internal Teams** referencing implementation details

## Technical Foundation
- **Framework**: Mintlify (docs-as-code)
- **Content Format**: MDX (Markdown + JSX components)
- **Config**: docs.json (navigation, theme, branding)
- **API Spec**: OpenAPI JSON (pi-reference/openapi.json)
- **Deployment**: Mintlify Dashboard (auto-deploy on push)
- **Theme**: Mint green (#16A34A primary)

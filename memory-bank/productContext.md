# Product Context: Raijin Labs Documentation

## Why This Project Exists

### The Problem Space

**Developer documentation is fragmented across Raijin Labs products:**
- Lucid-L2 API docs live in the repo README
- LucidMerged has internal docs/ folder but no public-facing guides
- OpenClaw integration specs are scattered across memory-bank files
- No unified place for developers to find API references, quickstarts, or tutorials

**Existing docs are internal-only:**
- Memory bank files are great for AI context but not for human developers
- Architecture docs in LucidMerged/docs/ are implementation-focused, not user-focused
- No interactive API explorer or code playground

### Our Solution: Mintlify Documentation Site

**Unified public documentation** for all Raijin Labs products:
- Single URL for all documentation
- Auto-generated API reference from OpenAPI specs
- Interactive code examples
- AI tool integration (Cursor, Claude Code, Windsurf)
- Search across all docs

## Problems We Solve

### For External Developers
- **Quick Onboarding**: Get from zero to first API call in < 2 minutes
- **API Reference**: Auto-generated, always up-to-date OpenAPI docs
- **Code Examples**: Copy-paste snippets in multiple languages
- **AI Integration**: Use docs directly in Cursor, Claude Code, Windsurf

### For Internal Teams
- **Single Source of Truth**: One place for all public documentation
- **Version Control**: Git-based, PR-reviewed content changes
- **Auto-Deploy**: Push to main = live in production
- **Consistent Branding**: Mintlify handles design/UX

## How It Should Work

### Developer Journey
1. Land on docs homepage
2. Click Quickstart
3. Get API key from dashboard
4. Make first API call (< 2 minutes)
5. Explore API reference for advanced features
6. Use AI tools for code generation

### Content Creation Workflow
1. Write MDX content locally
2. Preview with `mint dev` (localhost:3000)
3. Create PR on GitHub
4. Review and merge
5. Auto-deploys to production

## User Experience Goals

### Core Principles
1. **Speed**: Find answers in < 30 seconds
2. **Clarity**: No jargon, progressive disclosure
3. **Interactive**: Code examples you can copy and run
4. **Searchable**: Full-text search across all docs
5. **Beautiful**: Clean, modern design (Mintlify default)

### Design Language
- **Theme**: Mint green (#16A34A primary)
- **Layout**: Two-tab structure (Guides + API Reference)
- **Components**: Cards, columns, code blocks, callouts
- **Navigation**: Tab-based with sidebar groups

# Memory Bank Overview

This Memory Bank contains comprehensive documentation for the Raijin Labs Documentation project (C:\docs), designed to provide complete context after memory resets.

## File Structure

### Core Files (Required)
1. **`projectbrief.md`** - Foundation document defining project scope and requirements
2. **`productContext.md`** - Why this project exists, problems it solves
3. **`systemPatterns.md`** - Technical architecture and content patterns
4. **`techContext.md`** - Technologies, dev setup, deployment
5. **`activeContext.md`** - Current work focus and recent changes
6. **`progress.md`** - What works, what is left to build, current status

### File Relationships
```
projectbrief.md (foundation)
├── productContext.md (why & how)
├── systemPatterns.md (architecture)
└── techContext.md (technology)
    └── activeContext.md (current state)
        └── progress.md (status & next steps)
```

## Quick Reference

### Project Status (February 2026)
- **Overall Progress**: ~15% (scaffolding complete, content needed)
- **Current Focus**: Initialize memory bank and plan content customization
- **Infrastructure**: Mintlify fully deployed and auto-deploying
- **Content**: Still using starter kit defaults - needs full customization

### Technology
- **Platform**: Mintlify (docs-as-code)
- **Content**: MDX (Markdown + JSX)
- **Deployment**: Auto-deploy on push to main via Mintlify GitHub app
- **API Docs**: Auto-generated from OpenAPI spec

### Key Commands
```bash
npm i -g mint    # Install Mintlify CLI
mint dev         # Local preview at localhost:3000
mint update      # Update CLI
```

## Usage
Read all Memory Bank files at the start of each session to understand project context and continue work effectively.

**Last Updated:** February 19, 2026

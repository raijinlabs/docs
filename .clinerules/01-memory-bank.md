# Memory Bank Structure & Maintenance

## Memory Bank Overview

The Memory Bank consists of core files in Markdown format. Files build upon each other in a clear hierarchy.

## Core Files (Required)

### 1. projectbrief.md
- Foundation document that shapes all other files
- Created at project start if it does not exist
- Defines core requirements and goals
- Source of truth for project scope

### 2. productContext.md
- Why this project exists
- Problems it solves
- How it should work
- User experience goals

### 3. systemPatterns.md
- System architecture
- Key technical decisions
- Design patterns in use
- Component relationships
- Critical implementation paths

### 4. techContext.md
- Technologies used
- Development setup
- Technical constraints
- Dependencies
- Tool usage patterns

### 5. activeContext.md
- Current work focus
- Recent changes
- Next steps
- Active decisions and considerations
- Important patterns and preferences
- Learnings and project insights

### 6. progress.md
- What works
- What is left to build
- Current status
- Known issues
- Evolution of project decisions

## File Hierarchy

```
projectbrief.md (Foundation)
    ├── productContext.md (Why/What)
    ├── systemPatterns.md (How/Architecture)
    └── techContext.md (With What)
            └── activeContext.md (Current Focus)
                    └── progress.md (Status)
```

## Documentation Updates

Memory Bank updates occur when:
1. Discovering new project patterns
2. After implementing significant changes
3. When user requests with **"update memory bank"** (MUST review ALL files)
4. When context needs clarification

## Update Process

When updating Memory Bank:

1. **Review ALL Files** - Even if some do not require updates
2. **Document Current State** - What has been completed, what is in progress
3. **Clarify Next Steps** - What needs to happen next
4. **Document Insights & Patterns** - New learnings, architectural decisions

Focus particularly on `activeContext.md` and `progress.md` as they track current state.

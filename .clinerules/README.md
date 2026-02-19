# Cline Rules Directory

This directory contains organized rules that Cline follows when working on this project. Rules are loaded automatically and enforced during all sessions.

## File Organization

### Core Rules (Load First)
- **00-context.md** - MANDATORY context loading (HIGHEST PRIORITY)
- **01-memory-bank.md** - Memory Bank structure and maintenance

### How Cline Uses These Rules

1. **At session start:** Cline reads all `.clinerules/*.md` files
2. **During work:** Follows patterns and constraints defined in rules
3. **At session end:** Updates Memory Bank as specified in rules

## Key Workflows

### Starting a Session
User says: **"follow your custom instructions"**

### Ending a Session
User says: **"update memory bank"**

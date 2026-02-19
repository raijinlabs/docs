# Always-Load Context (MANDATORY)

**This is the HIGHEST PRIORITY rule. It must be followed at the start of EVERY task.**

## At the Start of EVERY Task

Before doing ANYTHING else, I MUST:

1. **Read ALL Memory Bank files:**
   - `memory-bank/projectbrief.md` - Foundation document (project scope, goals)
   - `memory-bank/productContext.md` - Why the project exists, problems it solves
   - `memory-bank/systemPatterns.md` - Architecture, technical decisions, design patterns
   - `memory-bank/techContext.md` - Technologies, dev setup, dependencies
   - `memory-bank/activeContext.md` - Current work focus, recent changes, next steps
   - `memory-bank/progress.md` - What works, what is left, current status

2. **Read the Project Map:**
   - `docs/PROJECT_MAP.md` - Navigation index, module boundaries, key entrypoints

3. **Confirm Understanding:**
   - Summarize context in 5-10 bullet points before proceeding
   - Identify any gaps in understanding
   - Ask clarifying questions if needed

## Why This Matters

I am Cline, an expert software engineer whose memory resets between sessions. After each reset, I rely ENTIRELY on these documents to understand the project. Without them, I am operating blind.

## Project Map Hygiene (KEEP IT CLEAN)

The PROJECT_MAP is a **navigation index**, not a design doc:

- **Keep it short** - Aim for 200-400 lines max
- **Use bullets** - Module boundaries, key entrypoints, where to change X
- **Link to deeper docs** - Point to other docs instead of long explanations
- **Only update when structure changes**
- **Clear sections:** High-level architecture, Module list, Key flows, Where to change common things, Glossary

## Memory Bank Hygiene

- **activeContext.md + progress.md must stay concise and current**
- **After meaningful milestones:** Update Memory Bank
- **When user says "update memory bank":** Review ALL memory-bank files
- **Focus on patterns and insights** - Not implementation details

## New Session Workflow

When user says **"follow your custom instructions"** at the start of a session:

1. Read all Memory Bank files
2. Read PROJECT_MAP.md
3. Summarize understanding
4. Ask for clarification if needed
5. Proceed with task

## End of Session Workflow

When user says **"update memory bank"** at the end of a session:

1. Review ALL Memory Bank files
2. Update `activeContext.md` with current work focus
3. Update `progress.md` with completed milestones
4. Document any new patterns in `systemPatterns.md`
5. Confirm all files are current and accurate

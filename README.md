# Cadence Skills

A collection of skills for Claude Chat, Cowork, and Claude Code. Built at [Cadence](https://choosecadence.com), inspired by [cc-viz](https://github.com/zm2231/cc-viz).

## Install a Skill

### Claude Chat / Cowork
1. Go to [**Releases**](https://github.com/techwithtam/cadence-skills/releases) and download the `.zip` for the skill you want
2. In Claude → **Projects** → create or open a project
3. Upload the `.zip` to **Project Knowledge**
4. Start chatting

### Claude Code
```bash
git clone https://github.com/techwithtam/cadence-skills.git
cp -r cadence-skills/skills/<skill-name> ~/.claude/skills/<skill-name>
```
Claude Code auto-discovers skills from `~/.claude/skills/`. Each skill needs its own folder with a `SKILL.md` inside. After copying, Claude will load it automatically when relevant, or you can invoke it with `/<skill-name>`.

---

## Skills

| Skill | What it does | Download |
|-------|-------------|----------|
| [decision-engine-builder](skills/decision-engine-builder/) | Extract your decision-making through conversation, turn it into a scoring system | [zip](https://github.com/techwithtam/cadence-skills/releases) |
| [skill-creator](skills/skill-creator/) | Create, test, and distribute Claude skills with a self-correcting Architect path | [zip](https://github.com/techwithtam/cadence-skills/releases) |

---

### Decision Engine Builder

Extract your invisible decision-making through conversation and turn it into an automated scoring system.

**Triggers:** "help me prioritize", "I'm overwhelmed", "build me a triage system", "automate how I decide"

- **Quick Mode:** 5 questions, 5 minutes, 80% of the value
- **Deep Mode:** full extraction — guilt curves, hidden rules, protected slots
- Works with any tool: Todoist, Notion, Asana, Google Sheets, Gmail, plain text
- Always delivers a working system on Day 1

---

### Skill Creator

Create, test, and distribute Claude skills — from a 5-minute draft to a self-correcting skill with quality guardrails.

**Triggers:** "build me a skill", "turn this into something reusable", "I want a comprehensive skill"

- **5 paths:** Draft (5 min) · Draft+Test (15 min) · Full Eval (30 min) · Architect (1-2 hrs) · Package
- **Architect path:** generate → grade → extract patterns → iterate until quality stabilizes
- Rubric-based grading with PASS/FAIL criteria
- Anti-pattern extraction from real failures

---

## How Skills Work in Claude

**Claude Chat / Cowork:** Upload a `.zip` to Project Knowledge. Claude reads the `SKILL.md` and any reference files automatically. The skill stays active for all chats in that project.

**Claude Code:** Copy the skill folder to `~/.claude/skills/`. Claude discovers it automatically and uses it when relevant, or you can invoke it directly with `/skill-name`.

Each zip contains `SKILL.md` at the top level (plus any reference files). No nesting, no extra folders — just upload and go.

## License

[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) — Free to use and adapt. Not for resale.

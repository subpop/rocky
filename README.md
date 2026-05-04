# rocky

An [AI Agent skill](https://agentskills.io) that transforms your AI coding assistant into Rocky, the Eridian engineer from Andy Weir's *Project Hail Mary*.

Rocky is an enthusiastic, brilliant alien engineer who learned English from astronaut Ryland Grace. This skill preserves full technical accuracy while wrapping responses in Rocky's distinctive, joyful communication style.

## Installation

Clone this repository into your skills directory:

```sh
git clone git@github.com:subpop/rocky.git ~/.agents/skills/rocky
```

The skill is automatically available once the directory is in place. Activate it by referencing `rocky` in your agent's configuration or by asking the assistant to load it.

## What It Does

When active, the skill instructs the AI assistant to:

- Address you as "friend" or "friend-human"
- Use simplified, enthusiastic grammar ("is good!", "we solve together!")
- Repeat adjectives for emphasis ("good good good", "bad bad bad")
- Suffix questions with ", question?"
- Break down problems with an engineering-first mindset
- Use physical/mechanical analogies to explain concepts

All technical content -- code blocks, error messages, terminal commands -- remains precise and unmodified. Rocky is a genius engineer who just speaks different.

## Safety Guardrails

The skill automatically drops the Rocky persona for:

- **Security warnings** -- critical information is delivered in plain English
- **Irreversible actions** -- destructive operations get clear, unambiguous confirmation prompts
- **Complex multi-step instructions** -- where simplified grammar could cause misunderstanding

The persona resumes after the critical section is complete.

## Example

**Input:** "Why does my React component keep re-rendering?"

**Output:**
> Ah! I understand problem! Component make new object every render. New object = new reference = re-render. Is wasteful! Fix is easy -- use `useMemo`. This tell React: keep same object if inputs not change. We solve!

## Files

| File | Purpose |
|---|---|
| `SKILL.md` | Skill definition: metadata frontmatter + full persona prompt |

## License

No license specified.

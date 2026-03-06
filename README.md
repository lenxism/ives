# ives

*In memory of Jony Ive — who showed us that design is how it works.*

A complete design philosophy and practical UI knowledge system for building exceptional interfaces. 13 composable skills that give AI coding agents the ability to reason about design — not just follow rules.

**Works with:** Claude Code, Cursor, Codex, OpenCode, Amp, and any tool supporting the [Agent Skills](https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) open standard.

## What makes this different

Every other design skill in the market falls into one of four categories:
- **Rule-based linters** — "your code violates these design rules"
- **Post-processing fixers** — "clean up the slop after generation"
- **Design memory systems** — "remember and enforce your choices"
- **Reference databases** — "query this catalog of good design"

**ives** is the layer underneath all of them: **design reasoning**. It teaches the agent *how to think about design contextually* — not just what to do, but *why*, and *when* it matters.

A real designer doesn't apply the same rules to a dense data dashboard and a luxury landing page. They reason about information density, user intent, visual hierarchy relative to content. This skill set encodes that reasoning.

## Architecture

### Tier 1: Craft Process (how to work)

| Skill | Purpose |
|-------|---------|
| **craft-philosophy** | Foundational mindset: noticing, uncommon care, less but better, live tuning |
| **design-critique** | Structured 4-lens review: visual design, interface design, interaction consistency, user context |
| **interface-architecture** | Structural decisions: platform defaults, information architecture, visual language |
| **conceptual-exploration** | Creative process: range (breadth of ideas) and depth (pushing a direction) |
| **quality-facets** | Quality measurement: define, evaluate, and track what "good" means for your product |
| **refinement-playbook** | Iteration process: remove redundancy → simplify → tighten → consistency → hierarchy → craft |

### Tier 2: Design Knowledge (what good looks like)

| Skill | Purpose |
|-------|---------|
| **typography** | Type sizes, weight as meaning, hierarchy, system fonts, the rule of four |
| **layout-spacing** | Box model, grids, negative space, alignment, density, spacing systems |
| **color** | Palettes, contrast/a11y, gray systems, dark UI, structural vs interactive color |
| **style-direction** | Corner radius, shadows, borders, opacity, buttons, design direction |
| **imagery** | Photos, icons, illustrations, app icons, dynamic images |
| **elements-patterns** | Navigation, inputs, forms, lists/cards, modals, tables, detail views |
| **tactics** | No-stress process, wireframes, responsive, platform guidelines, handoff |

## Installation

### Claude Code (plugin)

```bash
/plugin marketplace add your-username/ives
```

### Claude Code (manual)

```bash
git clone https://github.com/your-username/ives.git
cp -r ives/skills/* ~/.claude/skills/
```

### Cursor / Other tools

Copy the skill files into your project's prompt or context directory. The SKILL.md format is compatible with 40+ AI coding tools that support markdown-based instructions.

## How it works

The skills use **progressive disclosure** — only the skill name and description are loaded at startup (~100 words each). The full skill body is loaded only when relevant. Reference files with deep knowledge are loaded on-demand.

This means all 13 skills add minimal overhead to your context window while being available whenever design decisions arise.

### Typical flows

**Building something new:**
1. `craft-philosophy` loads as baseline mindset
2. `conceptual-exploration` helps explore before committing
3. `interface-architecture` guides structural decisions and visual language
4. `typography`, `color`, `layout-spacing` provide domain knowledge
5. `design-critique` runs self-critique before presenting

**Improving something existing:**
1. `design-critique` identifies specific issues
2. `quality-facets` measures and prioritizes
3. `refinement-playbook` systematically resolves
4. Domain skills (typography, color, etc.) provide specific guidance

**Quick review:**
1. `design-critique` runs the 4-lens framework
2. `quality-facets` if structured evaluation is needed

## Composability

**ives** is designed to work alongside other tools:
- Use with **rams.ai** for automated accessibility rule checking
- Use with **ui-skills** for post-generation fixes
- Use with **interface-design** for design memory/persistence
- Use with **Anthropic's frontend-design skill** for aesthetic steering

This skill set provides the *reasoning* layer that makes all of those tools more effective.

## Philosophy

> "Sometimes magic is just someone spending more time on something than anyone else might reasonably expect." — Penn & Teller

Most AI-generated interfaces stop at level 3 on a 1-10 quality scale. Not because the AI isn't capable of level 7+, but because nobody taught it to push further. **ives** encodes the mindset, knowledge, and process to close that gap.

## Contributing

This is an open-source project. Contributions welcome:
- Additional domain knowledge (animation, micro-interactions, data visualization)
- Platform-specific guidance (SwiftUI, React Native, Flutter)
- Real-world examples and case studies
- Translations

## License

MIT

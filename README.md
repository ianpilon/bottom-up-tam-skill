# Bottom-Up TAM (a Claude Code skill)

A reusable skill for [Claude Code](https://claude.com/claude-code) that walks you through building a defensible bottom-up TAM (total addressable market) for a startup pitch.

A "skill" is a self-contained instruction set that Claude Code auto-invokes when you say certain trigger phrases. Drop the folder into your skills directory and it becomes available in every project.

## What it does

Instead of pulling a top-down number from a McKinsey report ("recruiting is a $300B market, we'll get 1%"), this skill walks you through the bottom-up formula:

> **TAM = ACV (annual contract value) × number of customers in your ICP**

Then it shows the path to $10M ARR and $100M ARR (the venture-scale benchmark), runs a credibility check against common anti-patterns, and structures the output as a pitch-ready story.

It handles five different business models:

- **B2B high-ACV** (simple math, fast to scale)
- **B2C low-ACV** (counter the scary customer count with beachhead percentage)
- **Marketplace** (transactions, not customers; both sides of supply/demand)
- **Tiered or usage + subscription** (weighted ACV across tiers)
- **Multiple ICPs** (justify with cold-call conversion data, not convenience)

## Install

1. Clone or download this repo.
2. Copy the `bottom-up-tam/` folder into your Claude Code skills directory:

   ```bash
   cp -r bottom-up-tam ~/.claude/skills/
   ```

3. That is the whole install. Open Claude Code in any project and the skill is available.

## Use

Type `/bottom-up-tam` directly, or use one of the trigger phrases:

- "size this market"
- "draft a TAM slide"
- "is this venture scale"
- "what's the TAM for ..."
- "market sizing"

Claude will ask for the six inputs it cannot invent (product, ACV, ICP, customer count with source, business model, go-to-market), then produce the math and the pitch structure.

## Credit

The framework comes from a Launch accelerator talk by Kabir (This Week in Startups investment team), May 19 2026. The skill turns the talk into a repeatable workflow.

## License

MIT.

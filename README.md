# Heista Skills for Claude Code

Creative intelligence skills for Claude Code, powered by the Heista MCP server. Decode any video ad, load any brand, generate hooks, write scripts — all from inside Claude.

**MCP server:** `https://www.heista.co/api/mcp/mcp`
**API docs:** [heista.co/docs](https://heista.co/docs)
**Browse skills:** [heista.co/heista-skills](https://heista.co/heista-skills)

## Install

```bash
/plugin marketplace add Heista-co/claude-code-skills
/plugin install heista-decode@heista-skills
```

To install other skills, swap `heista-decode` for any plugin name below.

## Available skills

### `heista-decode`
Decode any video ad URL into a beat-by-beat structural breakdown — hooks, psychology, visual playbook, creative format. Use as raw material for new scripts, briefs, or moodboards.
**Costs credits** — token-metered through the Heista MCP.

### `heista-powersource`
Load any brand from a URL, internal documents (PDF, DOCX, briefs, brand guidelines, customer research), or both combined. Returns brand voice, buyer profile, behavioral tensions, marketing angles, selling points, proof, and narrative direction. The strategic foundation every script, hook, and brief is built from.
**Costs credits** — 100 credits URL or docs, 200 credits combined. Same-domain re-runs by the same org are free.

### `heista-hooks`
Generate video ad hooks backed by Heista's decoded corpus. Filter by vertical, hook type, or marketing angle. Returns proven shells, real example hooks, cadence profiles, runtime stats.
**Free** — corpus reads only.

### `heista-adscript`
Write video ad scripts on top of clustered formula blueprints from real winning ads. Pulls structure from the free formula corpus and decoded-ad library, then lets Claude write the copy from the user's context.
**Free** — uses corpus intelligence only.

### `heista-workflow-adscript`
Full chain: decode a competitor ad → load your brand → generate production scripts on the decoded structure in your brand's voice. One command for the whole pipeline.
**Costs credits** — chains paid decode + paid PowerSource + paid script generation.

## How it works

Skills bring procedural knowledge — *when* and *how* to use the underlying MCP tools. The MCP server at `heista.co/api/mcp/mcp` provides the actual tools (`decode_ad`, `create_powersource_url|docs|full`, `generate_adscript`, plus three free intelligence reads and `check_balance`). Authentication is OAuth on first use, or an API key from [heista.co/api-console](https://heista.co/api-console) for headless setups.

Full tool reference: [heista.co/docs § MCP](https://heista.co/docs#mcp).

## Account & credits

A Heista account is required for paid skills. Free skills work without one for the corpus reads, but `check_balance` and any paid call need an account.

- Sign up: [heista.co](https://heista.co)
- Top up: [heista.co/api-console/billing](https://heista.co/api-console/billing) — packs from $10 (500 credits) to $100 (12,500 credits)
- Manage API keys: [heista.co/api-console/keys](https://heista.co/api-console/keys)

## Source & support

- Repo: [github.com/Heista-co/claude-code-skills](https://github.com/Heista-co/claude-code-skills)
- API console: [heista.co/api-console](https://heista.co/api-console)
- Support: [support@heista.co](mailto:support@heista.co)
- Changelog: [CHANGELOG.md](./CHANGELOG.md)

Skills are MIT-licensed (see [LICENSE](./LICENSE)). The Heista MCP and API have their own terms at [heista.co/terms](https://heista.co/terms).

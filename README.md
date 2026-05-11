# Heista Skills for Claude Code

Creative intelligence skills for Claude Code, powered by the Heista MCP server. Decode any video ad, generate hooks from real winning patterns, write scripts in any brand's voice — all from inside Claude.

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

### `heista-hooks`
Generate video ad hooks backed by Heista's decoded corpus. Filter by vertical, hook type, or marketing angle. Returns proven shells, real example hooks, cadence profiles, runtime stats.
**Free** — corpus reads only.

### `heista-adscript`
Write video ad scripts on top of clustered formula blueprints from real winning ads. Pulls structure from the free formula corpus and decoded-ad library, then lets Claude write the copy from the user's context.
**Free** — uses corpus intelligence only.

### `heista-workflow-adscript`
Full chain: decode a competitor ad → extract brand intelligence (PowerSource) → generate production scripts on the decoded structure in the brand's voice. One command for the whole pipeline.
**Costs credits** — chains paid decode + paid PowerSource + paid script generation.

## How it works

Skills bring procedural knowledge — *when* and *how* to use the underlying MCP tools. The MCP server at `heista.co/api/mcp/mcp` provides the actual tools (decode_ad, create_powersource_*, generate_adscript, plus three free intelligence reads). Authentication is OAuth on first use, or an API key from [heista.co/api-console](https://heista.co/api-console) for headless setups.

## Source & support

- Repo: [github.com/Heista-co/claude-code-skills](https://github.com/Heista-co/claude-code-skills)
- API console: [heista.co/api-console](https://heista.co/api-console)
- Support: [support@heista.co](mailto:support@heista.co)

Skills are MIT-licensed. The Heista MCP and API have their own terms at [heista.co/terms](https://heista.co/terms).

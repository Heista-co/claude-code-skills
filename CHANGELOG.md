# Changelog

All notable changes to Heista skills are documented here. The marketplace follows [Semantic Versioning](https://semver.org/) per plugin.

## 2026-05-11

### Added
- `heista-powersource` plugin (v1.0.0) — load any brand from a URL, internal docs, or both. Voice, buyer profile, tensions, angles, and proof.

### Changed
- All five plugins polished for production: per-plugin `version`, `category`, `tags`, `author`, `homepage` in marketplace.json.
- Tightened skill copy to remove internal pipeline terminology.
- `LICENSE` file added (MIT).

### Fixed
- MCP tool prefix in every SKILL.md `allowed-tools` block now uses `mcp__heista__*` (Claude Code naming) instead of the cloud-app prefix. Skills can now actually gate tools when installed via Claude Code.

## 2026-05-04

### Added
- `heista-hooks` plugin (v1.0.0) — generate hooks from the decoded corpus. Free.
- `heista-adscript` plugin (v1.0.0) — write scripts on top of formula blueprints. Free.
- `heista-workflow-adscript` plugin (v1.0.0) — full chain: decode + brand load + script generation.

## 2026-05-02

### Added
- Initial release: `heista-decode` plugin (v1.0.0) — decode any video ad URL into structural formula, psychology, and creative intelligence.
- Marketplace registry, README.

[Repo](https://github.com/Heista-co/claude-code-skills) · [API docs](https://heista.co/docs) · [Browse skills](https://heista.co/heista-skills)

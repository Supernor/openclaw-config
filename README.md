# openclaw-config

Infrastructure state and configuration management for an [OpenClaw](https://github.com/openclaw/openclaw) deployment on a Hostinger VPS.

## What's here

| Directory | Contents |
|-----------|----------|
| `env/` | `.env.template` (redacted, no real secrets) |
| `config/` | Redacted `openclaw.json` structure |
| `logs/` | `ERRORS.md`, `LAST_RUN.md` — operational log summaries |
| `.github/` | GitHub Actions workflows |

## Config Versioning

Every config change is tracked via `config-tag.sh`, creating git tags for easy rollback. The `config-audit.jsonl` log inside the container records every write to `openclaw.json` with before/after hashes.

## Security

- No real secrets are stored in this repo
- `.env.template` shows key names with `REDACTED` values
- `openclaw.json` is stored in redacted form showing structure only
- Runtime secrets are injected via Docker Compose environment variables

## AI Attribution

All code in this repository was written by **Claude Code** (Anthropic's CLI agent), powered by **Claude Opus 4.6**.

- Human: Robert Supernor — product direction, priorities, review
- AI: Claude Code — implementation, architecture, infrastructure design

Every commit includes:
```
Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
```

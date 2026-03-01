# openclaw-config

Infrastructure state for the OpenClaw deployment on Hostinger VPS.

## Files

| File | Description |
|------|-------------|
| `.env.template` | Required env var names (no values) |
| `openclaw.json.structure` | Full config structure with credentials redacted |
| `auth-profiles.shape.json` | Auth profile shape with credentials redacted |
| `logs/LAST_RUN.md` | Last Repo-Man operation log |
| `logs/ERRORS.md` | WARN+ error log |
| `logs/DECISIONS.md` | Infrastructure decisions log |

## Security

- **No real secrets** are stored in this repo
- `.env.template` has variable names only
- `openclaw.json.structure` has REDACTED markers where secrets belong
- `auth-profiles.shape.json` has CREDENTIALS_REDACTED for all auth data

## Maintained By

- Repo-Man (env-backup skill) — pushes .env.template updates
- Claude Code — pushes config structure updates

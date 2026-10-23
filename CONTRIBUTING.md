# Contributing to this fork

This repository is StuxAPIs' hosted fork of [hnthap/lunar-calendar-api](https://github.com/hnthap/lunar-calendar-api).

- For changes to the API's actual behaviour (calendar conversion logic, new
  endpoints, bug fixes in `src/`), please contribute upstream first at
  [hnthap/lunar-calendar-api](https://github.com/hnthap/lunar-calendar-api/pulls)
  — this fork periodically pulls in upstream changes.
- For anything specific to how StuxAPIs hosts or deploys this fork
  (`Dockerfile`, `docker-compose.yaml`, `netlify.toml`, this fork's
  `README.md` branding, or its release files), open a pull request here
  directly.

## Local setup

```bash
npm install
npm run dev
```

See the upstream [README.md](README.md) for full API usage and environment
details.

## Questions

Reach out at [hello@stuxapis.net](mailto:hello@stuxapis.net).

## Versioning

This project uses [Date Versioning](https://datevers.ing). To release:

1. Add a `## vYY.MM.DD` entry at the top of `CHANGELOG.md`, with its sections in this order: Added, Changed, Fixed, Removed, Security, Deprecated.
2. Set `VERSION.md` to the same bare version (no `v`): today's **UTC** date as `YY.MM.DD`, or `YY.MM.DD-1`, `-2`… for later releases the same UTC day. Never a future date. Use UTC, not local time: just after midnight in the UK it is still the previous day in UTC.
3. Run `bash tests/version.sh`.
4. Run `./commit.sh` (or `commit.bat` on Windows). It checks the version, commits and tags `vYY.MM.DD`, and never pushes.

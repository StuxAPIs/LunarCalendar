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

## Releases

Releases follow [Semantic Versioning](https://semver.org/):

1. Update [CHANGELOG.md](CHANGELOG.md) with what changed.
2. Bump [VERSION.md](VERSION.md).
3. Run `commit.sh` (or `commit.bat` on Windows) to commit and tag the release.

## Questions

Reach out at [hello@stuxapis.net](mailto:hello@stuxapis.net).

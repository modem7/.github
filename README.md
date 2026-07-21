# .github

Account-wide defaults, consumed by two independent GitHub mechanisms:

- **`.github/settings.yml`** — read by the [Repository Settings App](https://github.com/apps/settings).
  Any repo without its own `settings.yml` inherits this file automatically. A repo with its own
  file needs `_extends: .github` to merge with it instead of replacing it outright (label arrays
  merge by `name`; other keys don't auto-merge — see
  [repository-settings/app's docs](https://github.com/repository-settings/app/blob/main/docs/configuration.md)).
- **`.github/FUNDING.yml`** — a native GitHub [community health file default](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file):
  any repo without its own `FUNDING.yml` picks this one up for its sponsor button.

Renovate presets live in a separate repo: [modem7/renovate-config](https://github.com/modem7/renovate-config).

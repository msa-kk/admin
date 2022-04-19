# safe-settings

[Safe-settings](https://github.com/github/safe-settings)– an app to manage
policy-as-code and apply repository settings to repositories across an
organization.

`admin`, `.github`, and `safe-settings` are ignored by default.

## Getting Started

Applies global and repository settings:

- Global settings across all repositories using
  [`.github/settings.yml`](../../.github/settings.yml).
- Override or add additional config for each repository file at [folder
  `.github/repos`](../../.github/repos/).

## Deployment

Deployed on k8s.

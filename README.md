# Renovate pre-commit hooks

A [pre-commit](https://pre-commit.com/) hook
to run [`renovate-config-validator`](https://docs.renovatebot.com/config-validation/#config-validation)
when you [reconfigure Renovate via PR](https://docs.renovatebot.com/getting-started/installing-onboarding/#reconfigure-via-pr).

Even though it is a Node-based hook, it works [without any system-level dependencies](https://pre-commit.com/#node).

## Usage

For general usage:

```yaml
repos:
  - repo: https://github.com/renovatebot/pre-commit-hooks
    rev: 38.128.6
    hooks:
      - id: renovate-config-validator
```

Or for a tighter configuration,
opt into [strict mode](https://docs.renovatebot.com/config-validation/#strict-mode):

```yaml
repos:
  - repo: https://github.com/renovatebot/pre-commit-hooks
    rev: 38.128.6
    hooks:
      - id: renovate-config-validator
        args: [--strict]
```

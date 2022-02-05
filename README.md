# Renovate pre-commit hooks

A [pre-commit](https://pre-commit.com/) hook to run `renovate-config-validator` when you [reconfigure Renovate via PR](https://docs.renovatebot.com/getting-started/installing-onboarding/#reconfigure-via-pr).

Even though it is a Node-based hook, it works [without any system-level dependencies](https://pre-commit.com/#node).

## Usage

```yaml
repos:
  - repo: github.com/maxbrunet/pre-commit-renovate
    rev: 31.66.6
    hooks:
      - id: renovate-config-validator
```

# nix-lefthook-brakeman

[![CI](https://github.com/pr0d1r2/nix-lefthook-brakeman/actions/workflows/ci.yml/badge.svg)](https://github.com/pr0d1r2/nix-lefthook-brakeman/actions/workflows/ci.yml)

> This code is LLM-generated and validated through an automated integration process using [lefthook](https://github.com/evilmartians/lefthook) git hooks, [bats](https://github.com/bats-core/bats-core) unit tests, and GitHub Actions CI.

Lefthook-compatible [Brakeman](https://github.com/presidentbeef/brakeman) security scanner hook for pre-push.

## Usage

Add to your `lefthook.yml`:

```yaml
remotes:
  - git_url: https://github.com/pr0d1r2/nix-lefthook-brakeman
    ref: main
    configs:
      - lefthook-remote.yml
```

## Development

```bash
nix develop
bats --recursive tests/unit/
```

## License

MIT

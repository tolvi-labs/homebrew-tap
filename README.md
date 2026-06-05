# homebrew-tap

Homebrew tap for [Tolvi Labs](https://tolvilabs.com) — install the `tolvi` CLI on macOS and Linux via Homebrew.

## Install

```bash
brew tap tolvi-labs/tap
brew install --cask tolvi-labs/tap/tolvi
```

Verify:

```bash
tolvi version
# v0.1.2
```

## What's in this tap

| Cask | Description |
|---|---|
| `tolvi` | Engineering knowledge vault CLI - capture decisions, sessions, and patterns as Markdown |

## Usage

After installing `tolvi`, initialize a vault in any repo:

```bash
export ANTHROPIC_API_KEY=sk-ant-...
tolvi init
tolvi sync decision "Why we chose Postgres"
tolvi ask "what did we decide about Postgres?"
```

Full docs at [tolvilabs.com/docs](https://tolvilabs.com/docs).

## Updating

```bash
brew upgrade --cask tolvi
```

The cask in this tap is updated automatically on each [tolvi release](https://github.com/tolvi-labs/tolvi/releases).

## Source

- CLI source: [github.com/tolvi-labs/tolvi](https://github.com/tolvi-labs/tolvi)
- Cask formula: [`Casks/tolvi.rb`](./Casks/tolvi.rb)

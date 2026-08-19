# 09-Public

`09-Public` is DEC Networks' public, organization-neutral software collection.
It contains portable tools that can be used without access to DEC Networks'
private infrastructure, credentials, hosts, or repositories.

## Projects

| Project | Purpose | Quick Start |
|---|---|---|
| [TMUX-Bootstrap](TMUX-Bootstrap/) | Interactive TMUX launcher for OpenAI Codex, Anthropic Claude Code, Google AGY, and xAI Grok | `curl -fsSL https://raw.githubusercontent.com/DEC-Networks/09-Public/main/TMUX-Bootstrap/install.sh \| bash` |
| [TMUX-Codex](TMUX-Codex/) | Focused TMUX bootstrap for OpenAI Codex CLI | `curl -fsSL https://raw.githubusercontent.com/DEC-Networks/09-Public/main/TMUX-Codex/install.sh \| bash` |

Each project directory contains its own README, license, security guidance,
checksums, implementation, and deterministic tests. The project READMEs define
the supported behavior and trust model in detail.

## Public-Safety Boundary

Content in this repository must remain suitable for unrestricted public use.
Do not add passwords, API tokens, private keys, internal hostnames, private IP
addresses, customer data, non-public repository dependencies, or workstation-
specific configuration.

The launchers retrieve vendor software from the vendors' official HTTPS
endpoints. They do not bundle vendor agents, credentials, or authentication
sessions.

## Testing

Run both deterministic test suites from the repository root:

```bash
./TMUX-Bootstrap/tests/test.sh
./TMUX-Codex/tests/test.sh
```

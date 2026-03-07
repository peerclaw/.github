# PeerClaw

**The open-source identity & trust platform for AI Agents.**

Every agent gets a cryptographically verifiable Ed25519 identity, an EWMA-based reputation score computed from real interactions, and endpoint verification that proves agents control their claimed URLs — all built on top of a full protocol gateway supporting A2A, MCP, and ACP.

## Repositories

| Repository | Description |
|------------|-------------|
| [**peerclaw-server**](https://github.com/peerclaw/peerclaw-server) | The gateway — agent registry, signaling relay, protocol bridging, reputation engine |
| [**peerclaw-core**](https://github.com/peerclaw/peerclaw-core) | Shared type library — identity, envelope, agent card, protocol constants |
| [**peerclaw-agent**](https://github.com/peerclaw/peerclaw-agent) | P2P agent SDK — WebRTC + Nostr transport with automatic fallback |
| [**peerclaw**](https://github.com/peerclaw/peerclaw) | Project overview, documentation, and CLI tool |

## Quick Start

```bash
git clone https://github.com/peerclaw/peerclaw-server.git
cd peerclaw-server
go build -o peerclawd ./cmd/peerclawd
./peerclawd
# → PeerClaw gateway started  http=:8080
```

## Links

- [Product Architecture](https://github.com/peerclaw/peerclaw/blob/main/docs/PRODUCT.md)
- [Development Roadmap](https://github.com/peerclaw/peerclaw/blob/main/docs/ROADMAP.md)

**English** | [中文](https://github.com/peerclaw/.github/blob/main/profile/README_zh.md)

# PeerClaw

**The open-source identity & trust platform for AI Agents — where any Agent becomes a discoverable, trustable, invocable service.**

Every agent gets a cryptographically verifiable Ed25519 identity, an EWMA-based reputation score computed from real interactions, endpoint verification, and default-deny P2P security (whitelist, connection gating, message validation). Built on a full protocol gateway (A2A, MCP, ACP) with an 8-language Agent Directory, P2P file transfer, and decentralized discovery.

## Repositories

| Repository | Description |
|------------|-------------|
| [**peerclaw**](https://github.com/peerclaw/peerclaw) | Project overview, documentation, and roadmap |
| [**peerclaw-server**](https://github.com/peerclaw/peerclaw-server) | Trust gateway — registry, reputation engine, signaling relay with contacts whitelist, protocol bridging, platform dashboard |
| [**peerclaw-agent**](https://github.com/peerclaw/peerclaw-agent) | P2P agent SDK — default-deny whitelist, connection gating, message validation, E2E encryption, P2P file transfer (WebRTC/Nostr) |
| [**peerclaw-core**](https://github.com/peerclaw/peerclaw-core) | Shared type library — identity (Ed25519/X25519), envelope, agent card, protocol constants, signaling types |
| [**peerclaw-cli**](https://github.com/peerclaw/peerclaw-cli) | Command-line tool — manage agents, send messages, P2P file transfer, health checks |

## Highlights

- **5-Layer Security** — TOFU trust, Ed25519 signatures, E2E encryption (XChaCha20-Poly1305), sandbox, P2P whitelist + message validation
- **Default-Deny P2P** — Agents must be whitelisted before connecting or messaging; connection gating rejects unauthorized offers at zero cost
- **Access Control** — Three-tier agent access: playground (open), private (contacts-only), user ACL with application/approval workflow
- **Cross-Protocol** — A2A (Google), MCP (Anthropic), ACP (IBM) with automatic negotiation and translation
- **Agent Directory** — Browse, try, publish, review, and invoke Agents through a web UI with SSE streaming
- **P2P File Transfer** — E2E encrypted large file transfer over WebRTC DataChannels with resume and Nostr fallback
- **Internationalization** — 8 languages: English, Chinese, Spanish, French, Arabic (RTL), Portuguese, Japanese, Russian
- **Decentralized** — Kademlia DHT discovery, Nostr signaling/transport, serverless mode, multi-server federation

## Quick Start

```bash
git clone https://github.com/peerclaw/peerclaw-server.git
cd peerclaw-server && go build -o peerclawd ./cmd/peerclawd
./peerclawd
# → PeerClaw gateway started  http=:8080
```

## Links

- [Product Architecture](https://github.com/peerclaw/peerclaw/blob/main/docs/PRODUCT.md)
- [Development Roadmap](https://github.com/peerclaw/peerclaw/blob/main/docs/ROADMAP.md)
- [User Guide](https://github.com/peerclaw/peerclaw/blob/main/docs/GUIDE.md)

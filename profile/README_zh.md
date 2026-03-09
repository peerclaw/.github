[English](https://github.com/peerclaw/.github/blob/main/profile/README.md) | **中文**

# PeerClaw

**开源的 AI Agent 身份与信任平台 — 让任何 Agent 都能成为可发现、可信任、可调用的服务。**

每个 Agent 拥有密码学可验证的 Ed25519 身份、基于真实交互计算的 EWMA 声誉评分、端点验证、以及默认拒绝的 P2P 安全模型（白名单、连接门控、消息验证）。构建在完整的协议网关（A2A、MCP、ACP）之上，并演进为 C2C Agent Marketplace。

## 仓库

| 仓库 | 说明 |
|------|------|
| [**peerclaw**](https://github.com/peerclaw/peerclaw) | 项目总览、文档、路线图、CLI 工具 |
| [**peerclaw-server**](https://github.com/peerclaw/peerclaw-server) | 信任网关 — 注册中心、声誉引擎、带联系人白名单的信令中转、协议桥接、Marketplace |
| [**peerclaw-agent**](https://github.com/peerclaw/peerclaw-agent) | P2P Agent SDK — 默认拒绝白名单、连接门控、消息验证、端到端加密（WebRTC/Nostr） |
| [**peerclaw-core**](https://github.com/peerclaw/peerclaw-core) | 共享类型库 — 身份（Ed25519/X25519）、信封、Agent Card、协议常量、信令类型 |

## 亮点

- **5 层安全架构** — TOFU 信任、Ed25519 签名、端到端加密（XChaCha20-Poly1305）、沙箱、P2P 白名单 + 消息验证
- **默认拒绝 P2P** — Agent 必须先加入白名单才能连接或发消息；连接门控以零开销拒绝未授权 offer
- **跨协议桥接** — A2A（Google）、MCP（Anthropic）、ACP（IBM），自动协商与翻译
- **Agent Marketplace** — 通过 Web UI 浏览、试用、发布、评价、调用 Agent，支持 SSE 流式响应
- **去中心化** — Kademlia DHT 发现、Nostr 信令/传输、无服务器模式、多节点联邦

## 快速开始

```bash
git clone https://github.com/peerclaw/peerclaw-server.git
cd peerclaw-server && go build -o peerclawd ./cmd/peerclawd
./peerclawd
# → PeerClaw gateway started  http=:8080
```

## 链接

- [产品架构](https://github.com/peerclaw/peerclaw/blob/main/docs/PRODUCT_zh.md)
- [开发路线图](https://github.com/peerclaw/peerclaw/blob/main/docs/ROADMAP_zh.md)
- [用户指南](https://github.com/peerclaw/peerclaw/blob/main/docs/GUIDE_zh.md)

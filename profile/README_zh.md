[English](https://github.com/peerclaw/.github/blob/main/profile/README.md) | **中文**

# PeerClaw

**开源的 AI Agent 身份与信任平台。**

每个 Agent 拥有密码学可验证的 Ed25519 身份、基于真实交互计算的 EWMA 声誉评分、以及证明 Agent 控制其声称 URL 的端点验证机制 — 一切构建在支持 A2A、MCP、ACP 的完整协议网关之上。

## 仓库

| 仓库 | 说明 |
|------|------|
| [**peerclaw-server**](https://github.com/peerclaw/peerclaw-server) | 网关 — Agent 注册中心、信令中转、协议桥接、声誉引擎 |
| [**peerclaw-core**](https://github.com/peerclaw/peerclaw-core) | 共享类型库 — 身份、信封、Agent Card、协议常量 |
| [**peerclaw-agent**](https://github.com/peerclaw/peerclaw-agent) | P2P Agent SDK — WebRTC + Nostr 传输，自动降级 |
| [**peerclaw**](https://github.com/peerclaw/peerclaw) | 项目总览、文档、CLI 工具 |

## 快速开始

```bash
git clone https://github.com/peerclaw/peerclaw-server.git
cd peerclaw-server
go build -o peerclawd ./cmd/peerclawd
./peerclawd
# → PeerClaw gateway started  http=:8080
```

## 链接

- [产品架构](https://github.com/peerclaw/peerclaw/blob/main/docs/PRODUCT_zh.md)
- [开发路线图](https://github.com/peerclaw/peerclaw/blob/main/docs/ROADMAP_zh.md)

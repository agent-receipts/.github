# agent-receipts

**Verifiable receipts for autonomous AI agents.**

An open protocol for cryptographically signed action receipts — so you can prove what an AI agent did, when, and why.

## Repos

| Repo | Description |
|------|-------------|
| [ar](https://github.com/agent-receipts/ar) | Monorepo — protocol spec, SDKs (Go, TypeScript, Python), MCP proxy, docs site |
| [openclaw](https://github.com/agent-receipts/openclaw) | Agent Receipts plugin for OpenClaw |

## How it works

1. An AI agent performs actions through MCP or any tool-use protocol
2. Each action produces a **signed receipt** (Ed25519) with a canonical hash (RFC 8785 + SHA-256)
3. Receipts are **hash-chained** — forming a tamper-evident audit trail
4. Receipts can be stored, queried, verified, and exported

## Get started

```bash
# Python
pip install agent-receipts

# TypeScript
npm install @agnt-rcpt/sdk-ts

# Go
go get github.com/agent-receipts/ar/sdk/go
```

Docs at [agentreceipts.ai](https://agentreceipts.ai)

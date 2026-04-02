# agent-receipts

**Verifiable receipts for autonomous AI agents.**

An open protocol for cryptographically signed action receipts — so you can prove what an AI agent did, when, and why.

## What's here

| Repo | Description |
|------|-------------|
| [spec](https://github.com/agent-receipts/spec) | Protocol specification, JSON schemas, canonical action taxonomy |
| [sdk-ts](https://github.com/agent-receipts/sdk-ts) | TypeScript SDK |
| [sdk-py](https://github.com/agent-receipts/sdk-py) | Python SDK |
| [sdk-go](https://github.com/agent-receipts/sdk-go) | Go SDK |
| [mcp-proxy](https://github.com/agent-receipts/mcp-proxy) | MCP proxy — transparent governance + receipt signing for any MCP server |
| [site](https://github.com/agent-receipts/site) | Documentation site |

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
npm install agent-receipts

# Go
go get github.com/agent-receipts/sdk-go
```

Docs at [agentreceipts.ai](https://agentreceipts.ai)

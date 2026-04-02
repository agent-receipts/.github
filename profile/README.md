# agent-receipts

**Verifiable receipts for autonomous AI agents.**

An open protocol for cryptographically signed action receipts — so you can prove what an AI agent did, when, and why.

## What's here

Everything lives in a single monorepo: **[agent-receipts/ar](https://github.com/agent-receipts/ar)**

| Directory | Description |
|-----------|-------------|
| [`spec/`](https://github.com/agent-receipts/ar/tree/main/spec) | Protocol specification, JSON schemas, canonical action taxonomy |
| [`sdk/go/`](https://github.com/agent-receipts/ar/tree/main/sdk/go) | Go SDK |
| [`sdk/ts/`](https://github.com/agent-receipts/ar/tree/main/sdk/ts) | TypeScript SDK |
| [`sdk/py/`](https://github.com/agent-receipts/ar/tree/main/sdk/py) | Python SDK |
| [`mcp-proxy/`](https://github.com/agent-receipts/ar/tree/main/mcp-proxy) | MCP proxy — transparent governance + receipt signing for any MCP server |
| [`site/`](https://github.com/agent-receipts/ar/tree/main/site) | Documentation site |

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
npm install @agent-receipts/sdk-ts

# Go
go get github.com/agent-receipts/ar/sdk/go
```

Docs at [agentreceipts.ai](https://agentreceipts.ai)

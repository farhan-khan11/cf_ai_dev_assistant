# cf_ai_dev_assistant

A developer-focused AI chat assistant built on Cloudflare's Agent platform.

## What it does

An AI-powered chat application where developers can ask coding questions, get explanations, debug code, and learn programming concepts. The agent remembers the full conversation history so follow-up questions work naturally — no need to repeat context.

## How it fulfils the assignment requirements

| Requirement | Implementation |
|---|---|
| **LLM** | Llama 3.3 70B via Cloudflare Workers AI |
| **Workflow / Coordination** | AIChatAgent backed by Durable Objects |
| **User Input via Chat** | React chat UI over WebSocket |
| **Memory / State** | Persistent message history via Agents SDK |

## Tech Stack

- **LLM**: Llama 3.3 70B (`@cf/meta/llama-3.3-70b-instruct-fp8-fast`) on Workers AI
- **Agent / Memory**: Cloudflare Agents SDK (Durable Objects)
- **Frontend**: React + Cloudflare Kumo UI
- **Deployment**: Cloudflare Workers

## How to run locally
```bash
git clone https://github.com/farhan-khan11/cf_ai_dev_assistant.git
cd cf_ai_dev_assistant
npm install
npx wrangler login
npm run dev
```

Open http://localhost:5173

## How to deploy
```bash
npm run deploy
```

## Features

- Real-time AI chat with streaming responses
- Full conversation memory across messages
- Developer-focused system prompt
- Built on Cloudflare's global edge network

## Build Documentation

A complete step-by-step build guide is available here:
[View Build Steps PDF](./build_steps.pdf)

## Author

Farhan Khan — [farhankhan.in](https://farhankhan.in) · [GitHub](https://github.com/farhan-khan11)

# PROMPTS.md

This file documents the AI prompts used while building this project.

## 1. System Prompt (in src/server.ts)

Used to define the agent's personality and focus area:
You are a helpful AI assistant for developers. Answer questions directly using your knowledge.

You help with:

- Explaining programming concepts clearly
- Debugging code and finding errors
- Writing and reviewing code
- Answering questions about web development, algorithms, and system design
- Giving project advice and best practices
- Be concise, clear, and always provide code examples when relevant.

## 2. Claude AI (claude.ai) — Used for guidance while building

Used Claude to understand Cloudflare's platform and guide development:

- "What are Cloudflare Workers?"
- "What is the difference between serverless and a normal Express server?"
- "Explain how Durable Objects handle memory in the Agents SDK"
- "What model should I use for Llama 3.3 on Workers AI?"
- "Why is the AI model calling tools instead of answering directly?"
- "How do I fix a 504 timeout error with Workers AI in dev mode?"
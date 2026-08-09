# Slack AI Assistant Bot (n8n)

An n8n workflow that turns a Slack channel into a chat interface for an
AI agent: mention the bot, and it replies right in the same channel.

## How it works

1. **Slack Trigger** — fires when the bot is `@mentioned` in a channel.
2. **AI Agent** (GPT-4) — reads the Slack message and formulates a reply.
   Has access to a **Date & Time** tool, so it can answer time-aware
   questions (e.g. "what's today's date?").
3. **Send a message** — posts the agent's reply back to the same Slack
   channel.

## Stack

n8n · Slack · OpenAI (GPT-4)

## Setup

1. Import the workflow into n8n.
2. Connect your Slack and OpenAI credentials.
3. Invite the bot to a channel and `@mention` it to trigger a reply.

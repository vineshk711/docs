---
title: "Introduction"
description: "The Birdeye MCP server gives AI assistants direct access to your Birdeye data — reviews, listings, surveys, social, ticketing, search AI insights and more"
---

## What is the Birdeye MCP Server?

The **Birdeye MCP Server** implements the [Model Context Protocol (MCP)](https://modelcontextprotocol.io), an open standard that lets AI assistants (Claude, ChatGPT, and others) securely connect to external data sources and services.

By connecting your AI assistant to `https://mcp.birdeye.com/mcp`, you can ask natural-language questions and get real-time answers powered by your live Birdeye account data.

- [Quickstart](quickstart.md) — Connect your AI assistant to Birdeye in under 5 minutes
- [Authentication](authentication.md) — Learn how OAuth 2.0 keeps your data secure
- [Tools Reference](tools/overview.md) — Browse all 22 available tools by category
- [Birdeye Platform](https://birdeye.com) — Learn more about the Birdeye platform

## What can you do?

Once connected, your AI assistant can answer questions like:

- *"What are my review trends over the last 30 days?"*
- *"Which of my locations have the lowest listing accuracy on Google?"*
- *"Show me the SWOT analysis from the latest Search AI run."*
- *"How did my Facebook posts perform last month compared to the month before?"*

## Supported AI Clients

The Birdeye MCP Server is compatible with any MCP-capable AI client:

- **Claude** (claude.ai)
- **ChatGPT** (chatgpt.com)
- Any other MCP-compatible client

{% hint style="warning" %}
If you are using an MCP client other than ChatGPT or Claude, you must register it with Birdeye by providing your redirect URI to Birdeye Support.
{% endhint %}

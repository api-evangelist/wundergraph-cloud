---
title: "MCP Scope Step-Up Authorization: From Implementation to Spec Contribution"
url: "https://wundergraph.com/blog/mcp-scope-step-up-authorization"
date: "2026-03-05"
author: ""
feed_url: "https://wundergraph.com/rss.xml"
---
Cosmo's MCP server already exposes your graph as AI-ready tools. When we added per-tool OAuth scope step-up authorization so clients don't need a god token, we hit an infinite loop. The root cause: a gap between the MCP spec and RFC 6750 on scope challenges, plus SDK behavior that overwrites scopes instead of accumulating them. Here's what we found and how we're approaching it.

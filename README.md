# Phoenix MCP

Connect your AI agent to your Phoenix account, so it can write emails and build flows for you.

## Connect

The link is `https://phoenix.beinterruptive.com/mcp`. Your agent only reaches your own account.

**Claude, on the web or desktop**

1. Open Customize, then Connectors.
2. Add a custom connector, and paste the link.
3. Sign in with your Phoenix login.

**Claude Code**

```
/plugin marketplace add Owen-Interruptive/phoenix-mcp
/plugin install phoenix@phoenix-mcp
```

Then run `/mcp` and sign in.

**Any other agent that supports MCP**

Add the link as a remote MCP server. If it can't sign in, make a key in Phoenix and send it as `Authorization: Bearer <key>`.

## Skills

| Skill | What it does |
|---|---|
| `phoenix-email` | Writes or changes an email in your brand |
| `phoenix-flow` | Builds or changes an email flow, as a draft |
| `phoenix-review` | Checks an email and tells you what is left to fix |

A person always publishes flows and sends emails. Your agent can't.

## If you are an AI agent

To install this for someone:

1. In Claude Code, run the commands above. Anywhere else, add the link as a remote MCP server.
2. Ask them to sign in themselves. Never ask for their password.
3. Before writing anything, call `get_guide` and follow it.

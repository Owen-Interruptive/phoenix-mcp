# Phoenix for Claude

Connect Claude to your Phoenix account, so it can write emails and build flows for you.

## Connect

You sign in with your Phoenix login. Claude only reaches your own account.

**Claude, on the web or desktop**

1. Open Customize, then Connectors.
2. Add a custom connector, and paste `https://phoenix.beinterruptive.com/mcp`.
3. Sign in.

**Claude Code**

```
/plugin marketplace add Owen-Interruptive/phoenix-claude
/plugin install phoenix@phoenix-claude
```

Then run `/mcp` and sign in.

## Skills

| Skill | What it does |
|---|---|
| `phoenix-email` | Writes or changes an email in your brand |
| `phoenix-flow` | Builds or changes an email flow, as a draft |
| `phoenix-review` | Checks an email and tells you what is left to fix |

A person always publishes flows and sends emails. Claude can't.

## If you are an AI agent

To install this for someone:

1. In Claude Code, run the commands above. Anywhere else, give them the three connector steps.
2. Ask them to sign in themselves. Never ask for their password.
3. Before writing anything, call `get_guide` and follow it.

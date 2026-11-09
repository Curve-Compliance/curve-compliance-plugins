# Curve Compliance plugins

This repository holds the Curve Compliance plugin for Claude, in the `curve-compliance` folder. The plugin is for Curve Compliance customers: it connects Claude to your organisation's Curve account and adds skills for a weekly marketing report, campaign reviews, goals and attribution, website and search reports, and tracking checks. Answers are totals and breakdowns from your own Curve account, never records about a person.

The plugin's [README](curve-compliance/README.md) explains what you need before you start, how to connect on claude.ai, in Cowork and in Claude Code, and what data the connector sends and receives.

Add Curve Compliance from Claude's plugin directory. In Claude Code you can also add this repository as a plugin marketplace with `/plugin marketplace add Curve-Compliance/curve-compliance-plugins` and then install `curve-compliance`.

## Other AI tools

Each skill is a `SKILL.md` file in its own folder under `curve-compliance/skills/`, for agents that read skills from a GitHub repository. The skills answer only once the Curve Compliance connector is added.

Claude, ChatGPT, Grok, Cursor, Codex and Claude Code sign in to the connector through the same Curve sign-in page the [plugin README](curve-compliance/README.md#connect) describes. Setup notes for each are at https://www.curvecompliance.com/curve-mcp.

Any other tool that can add a remote MCP server with a token connects to https://mcp.curvecompliance.com/mcp with a personal token. You create it in Curve under **Marketing → Curve MCP**, on the card labelled **Claude Code**, whichever tool you use it with. If the card says "You cannot create a personal token from this login", ask the Curve team.

Questions: hey@curvecompliance.com.

Copyright 2026 Curve Technologies, Inc. d/b/a Curve Compliance. All rights reserved. See [LICENSE](LICENSE).

---
name: get-started
description: Introduce the Curve Compliance plugin and help the user connect it. Use when the user has just added the plugin, asks what it can do or how to connect it, or mentions Curve without giving a task.
---

Use this skill when the user has just added Curve Compliance, mentions it without a task, or asks what it can do or how to connect it.

## If the Curve tools are missing

If you have no `get_access_info` tool, the Curve Compliance connector is not connected yet. Tell the user how to connect, in a few short lines:

1. They need a Curve login in an organisation where the Curve team has turned on Curve MCP for Claude. Their **External AI tools** switch, on the **AI access** card under **Management → User Access**, must be on; the organisation's primary user can switch a person on.
2. On claude.ai and in Cowork, they open this plugin's **Connectors** tab and connect Curve Compliance. On Claude Team and Enterprise plans, an Owner adds the connector for the organisation first.
3. In Claude Code, they run `/mcp`, choose the Curve Compliance server and sign in.
4. Curve then opens a page in the browser. They sign in to Curve, check that the page names the right organisation, select **Allow**, and enter the code Curve emails them or the one from their authenticator app.

Then wait until the user says they are connected.

## If the Curve tools are there

1. If the connection reaches several client accounts, the Curve tools ask for an account. Ask the user which one first, and name it in every call.
2. Call `get_access_info`. It lists the reports that are ready for this account and the rules for reading every answer. Follow those rules for the rest of the conversation.
3. Reply in a few short lines:
   - One sentence: the plugin answers questions about the organisation's marketing with figures from its own Curve account.
   - Three questions the user could ask now, picked from the reports `get_access_info` lists as available. Last week's marketing report, compared with the week before, is a good first one.
   - A question about a specific person (a patient, lead or visitor) is asked in Curve itself, through a one-time link, and is never answered in the chat.
4. Do not call another tool until the user gives a task.

Explicit instructions from the user always take priority over this skill.

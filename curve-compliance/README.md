# Curve Compliance

For Curve Compliance customers. This plugin connects Claude to your organisation's Curve account, so you can ask about your marketing and get figures from your own Curve reports: last week's report compared with the week before, spend and conversions across Google Ads, Meta and your other connected ad platforms, website traffic, goals, forms, consent and search. Answers are totals and breakdowns, never records about a person.

## What it adds

The **Curve Compliance** connector, at https://mcp.curvecompliance.com/mcp. It gives Claude tools that read your Curve reports, and **Open this in Curve**, which makes a one-time link into Curve.

Six skills that tell Claude how to use those reports for everyday questions:

- `get-started` introduces the plugin and explains how to connect it.
- `weekly-marketing-report` gives a week's report against the week before and explains what changed.
- `campaign-review` compares campaigns, ad groups, ads and keywords on spend, conversions and cost per conversion.
- `goals-and-attribution` covers goals, the channels and campaigns behind them, funnels, forms and CRM outcomes.
- `website-and-search` covers traffic, landing pages, organic search, AI assistants, Google Business Profile and recorded visits.
- `tracking-health` checks conversion forwarding to your ad platforms, missing data and consent.

## Before you start

You need a Curve login in an organisation where the Curve team has turned on Curve MCP for Claude. Your **External AI tools** switch, on the **AI access** card under **Management → User Access**, must also be on. Your organisation's primary user can switch a person on or off.

## Connect

On claude.ai and in Cowork, open the plugin's **Connectors** tab and connect Curve Compliance. On Claude Team and Enterprise plans, an Owner adds the connector for the organisation first, and each person then connects with their own Curve login.

In Claude Code, run `/mcp`, choose the Curve Compliance server and sign in.

Either way, Curve opens a page in your browser. Sign in to Curve, check that the page names your organisation, select **Allow**, and enter the code Curve emails you or the one from your authenticator app. If your login reaches several client accounts, Claude asks you which one to use before it asks for figures.

## Use it

Try, for example:

- "Give me last week's marketing report and what changed."
- "How did our Google Ads and Meta campaigns do over the last 30 days?"
- "Which goals did people complete most last month, and which channels drove the top one?"

Periods are complete days in your organisation's reporting timezone, so today is never included. A report your organisation has not set up in Curve says so instead of giving figures. Before an answer leaves Curve, small counts are not shown as exact numbers, names that look like personal details are hidden, and nothing about an individual patient, lead or visitor is returned. For a question about a specific person, Claude gives you a one-time link instead. You open it from your own Curve login, and it drafts the question in Curve AI, if your login can use Curve AI.

Nothing Claude asks can change your Curve settings, reports or ad accounts. Daily limits apply to requests and links, per person and per organisation.

## Data

This plugin holds instructions for Claude and the address of Curve's server. It runs no code on your computer and sends nothing to any other service.

Curve receives the tool calls Claude makes: which report, the period, and options such as a breakdown or a filter. When you ask about a specific person, Claude asks Curve for a link instead of figures, and that request can carry the question Claude drafted and the person's email address or phone number, if you gave one. Curve removes links, email addresses and phone numbers from the drafted question, and does not use the email address or phone number to look anyone up. Curve also receives the assistant's name and the network address of each request, for security checks. It does not receive the rest of your conversation.

Curve records every call, and you can see your calls under **Marketing → Curve MCP** in Curve. To disconnect Claude, use **Connected AI tools** in your Curve account menu. Section 1.E of the privacy policy, https://www.curvecompliance.com/privacy, says what Curve keeps and for how long.

## Support

Email hey@curvecompliance.com. Setup notes are at https://www.curvecompliance.com/curve-mcp.

## Licence

Copyright 2026 Curve Technologies, Inc. d/b/a Curve Compliance. All rights reserved. See [LICENSE](LICENSE).

# Sitesfare

Make, edit and publish a [Sitesfare](https://sitesfare.com) website from a conversation with Claude. Say what you
are making — "a website for my bakery in Pune" — and Sitesfare builds a complete site with your words in it. Then
change any text, photo or link, hide or add sections and buttons, pick colours and fonts, add functions to a wedding
site, and publish when you are happy. Every change is kept in the site's history and can be undone.

Sitesfare makes websites for businesses, portfolios, online stores, weddings and housing societies, hosted on
`yourname.sitesfare.app` with HTTPS. Drafting is free; the first website goes live free for 30 days, then stays live
with its plan.

## What is in this plugin

- **The Sitesfare connector** (`.mcp.json`): Sitesfare's own remote MCP server at `https://api.sitesfare.com/mcp`.
- **The skill `sitesfare-website`**: the order Claude works in — make the site, replace the design's sample words
  with yours, never invent reviews, numbers or addresses (those sections are hidden until you give real ones), ask
  for your photos, and publish only when you say so.

## Signing in

The first time Claude uses a Sitesfare tool, you sign in with your Sitesfare account on `sitesfare.com` (OAuth 2.1;
you can create a free account on that page). Claude never sees your password. You can disconnect at any time in
Claude's connector settings or under AI editors in the Sitesfare dashboard.

## What it sends and where

The plugin runs nothing on your computer. Claude calls the Sitesfare server at `https://api.sitesfare.com/mcp`
only, and only for what you ask: the words, links and photos you give for your site, and the changes you ask for.
Photos you add by link are fetched by Sitesfare from that link. Each call is recorded in your site's history and in
Sitesfare's audit log. Privacy policy: <https://sitesfare.com/privacy>. Terms: <https://sitesfare.com/terms>.

## Example requests

- "Make me a website for my bakery in Pune, called Kiln & Co"
- "Make a wedding website for Asha & Rohan, 18 November 2027 in Pune"
- "Change the opening hours on my website to 9am–7pm"
- "Hide the testimonials and publish my website"

## Install

- **Claude (claude.ai, desktop):** from the Claude directory, or add the connector `https://api.sitesfare.com/mcp`
  under Settings → Connectors.
- **Claude Code:** `/plugin marketplace add vistraal/sitesfare-for-claude`, then `/plugin install sitesfare@sitesfare`,
  and `/mcp` to sign in.

## Support

<https://sitesfare.com/contact> · Step-by-step guide: <https://sitesfare.com/guides/connect-claude>

Licence: the files of this plugin are MIT (see `LICENSE`). Sitesfare designs and the websites built from them are
licensed for hosting on Sitesfare only.

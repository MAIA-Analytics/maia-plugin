# MAIA plugin for Claude

[MAIA](https://www.maia-analytics.com) is a geospatial research engine for questions about places in the United States. Ask in plain language and MAIA's agent researches it and builds the answer as a project with a map and a table: which places or properties match your criteria, who owns them, what is near them, how many there are in an area, or a list of them with contacts or other details for each row.

Data can include parcels, owners, zoning, buildings, contacts, businesses and points of interest, schools, roads and land use. MAIA's agent can also find and add suitable public map layers.

## What the plugin contains

- **MAIA connector** (`.mcp.json`): connects Claude to MAIA's remote MCP server at `https://api.maia-analytics.com/mcp`. The first time you use it, Claude opens MAIA's sign-in page (OAuth). The plugin stores no credentials.
- **`maia` skill** (`skills/maia/SKILL.md`): tells Claude when to use MAIA and how to start a request.

The plugin runs no local code, scripts or hooks.

## Example requests

- Find industrial-zoned parcels over 1 acre in San Francisco
- Show me single-family lots over 7,500 sqft in West Seattle that haven't sold in 20+ years
- Who owns the vacant lots in SoMa, San Francisco?

## Data handling

The plugin sends your requests, and any file you ask Claude to import, to MAIA's server only. MAIA stores your projects in your MAIA account. See the [privacy policy](https://www.maia-analytics.com/privacy) and [terms](https://www.maia-analytics.com/terms).

## Setup and support

Setup guide: <https://www.maia-analytics.com/docs/mcp/connect>. Support: support@maia-analytics.com.

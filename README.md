# 442ball connector

[![442ball MCP connector on Glama: tool quality and endpoint health](https://glama.ai/mcp/connectors/com.442ball/442ball/badges/score.svg)](https://glama.ai/mcp/connectors/com.442ball/442ball)

442ball is a football publication at [442ball.com](https://442ball.com). This connector lets Claude and other AI assistants read 442ball's own weekly club Power Ratings and the ratings built on them. Every answer links to the 442ball page of each club and league it names.

**Address:** `https://mcp.442ball.com/mcp` (streamable HTTP, no sign-in)

**In Claude:** find 442ball in the connectors directory, or add the address above as a custom connector. Step-by-step guides for other assistants are at [442ball.com/en/ai](https://442ball.com/en/ai).

## The 12 tools, all read-only

- **resolve:** find a club or league by name
- **club_rating:** a club's latest Power Rating, band, league rank, attack and defence indices and long-run rating
- **compare_clubs:** two clubs side by side
- **league_strength:** a league's strength
- **rankings:** a league's clubs by rating
- **rating_history:** a club's rating month by month
- **method:** how the ratings are made
- **club_runs:** a club's current and longest runs: unbeaten, winning, winless, clean sheets
- **league_runs:** a league's longest current runs
- **movers:** the week's biggest risers and fallers
- **league_index:** the 442 League Index of European leagues
- **greatest_sides:** the best league seasons within one league since 2010/11

**Example questions:** "What is Liverpool's 442ball rating?" · "Compare Liverpool and Manchester City on 442ball." · "What is the greatest Premier League side on 442ball?"

## What it never returns

Scores, fixtures or results; lineups or player statistics; data or identifiers from our football data provider; predictions or odds of any kind.

## Limits, per network address

60 calls a minute, 600 an hour and 2,000 a day; 500 different clubs or leagues a day; 300 name lookups an hour; answers of up to 16 KB.

## How the ratings work

[442ball.com/en/ratings/method](https://442ball.com/en/ratings/method). They are recalculated every Monday from finished match results. They measure how strong results have been; they are not predictions.

## Privacy

The connector never sees your conversation. It keeps only a salted one-way code of the caller's network address and a 30-day call log, to apply its limits. Full notice: [mcp.442ball.com/privacy](https://mcp.442ball.com/privacy).

## Also listed in

The official MCP Registry as `com.442ball/442ball`.

## Contact

hello@442ball.com

This repository holds the connector's public listing information only. The connector is operated by Eduloom Technologies (OPC) Private Limited, publisher of 442ball.

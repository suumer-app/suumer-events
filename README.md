# Suumer events

[![Suumer MCP connector](https://glama.ai/mcp/connectors/com.suumer/events/badges/score.svg)](https://glama.ai/mcp/connectors/com.suumer/events)

Things to do near any US town on any day: trivia, live music, karaoke, open mics, markets and more. Each event is checked against the page it came from. Free, no key, no sign-in.

- Website: https://suumer.com (Suumer, with two U's)
- Open feed: https://suumer.com/api (fields in [openapi.json](https://suumer.com/openapi.json); use is covered by the [data terms](https://suumer.com/data-terms))
- For AI tools: https://suumer.com/mcp (MCP, streamable HTTP), listed in the official MCP Registry as `com.suumer/events`

## Try it

```
curl "https://suumer.com/api/v1/events?town=Columbus,%20OH&limit=5"
```

Send a town (`Tampa, FL`), a ZIP, or `lat` + `lon`. Add `from` and `to` (YYYY-MM-DD) for other days, `category` for one kind of event, `radius` in miles.

## Use it in an AI app

Add `https://suumer.com/mcp` as a remote MCP server (Claude, ChatGPT, Cursor, VS Code). Its tool `find_events` takes a place, dates, a kind of event and a radius.

Please link each event's Suumer page (`https://suumer.com/e/<id>`) when you show it.

Questions: hello@suumer.com

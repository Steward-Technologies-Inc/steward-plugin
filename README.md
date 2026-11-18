# Steward

Steward connects an AI assistant to your own Steward account: the cards in your wallet,
your saved card-linked offers, loyalty status and points. When you are deciding where to
buy something, which card to use, or whether to pay cash or points for a flight or hotel,
the assistant can read what applies to you and say which option comes out ahead and why.

Steward advises only. It never buys, books, activates an offer or transfers points.

## What is in this plugin

- A connection to Steward's hosted server at `https://api.stewardflow.com/mcp`. Nothing
  runs on your machine and the plugin contains no code.
- One skill, `steward-purchase-decisions`, that tells the assistant when Steward is
  relevant and how to present what it returns.

## What you need

A Steward account. Create one in the Steward app for iPhone, add the cards you carry, and
optionally your loyalty programmes and offers.

## Connect

The connection is not open to the public yet. When it is:

**Claude.** Settings, Connectors, Add custom connector, and enter
`https://api.stewardflow.com/mcp`. Once Steward is listed in Claude's directory you can
connect from there instead.

**ChatGPT.** Plugins, Add, create an MCP app with `https://api.stewardflow.com/mcp` as the
server URL and OAuth as the sign-in method. Once Steward is listed in ChatGPT's directory
you can connect from there instead.

Either way you are sent to Steward to sign in, then shown a list of what the assistant may
read, each with its own checkbox: wallet, offers, points, loyalty, trips, goals, spending
summaries, saved merchants and saved notes. Untick anything you do not want to share and
press Allow. Nothing is shared before that.

## Things to ask

- "Which of my cards should I use at Whole Foods?"
- "I'm buying a $900 TV. Is Best Buy or Amazon better with my cards?"
- "Do I have any card offers expiring this month?"
- "How much are the points I have on my cards worth right now?"
- "Which of my card credits haven't I used this year?"

## Disconnect

In the Steward app, open Connected Assistants and remove the assistant. Access ends
immediately. You can also disconnect from the assistant's own settings.

## Privacy

What Steward collects, what an assistant can receive, how long it is kept and who it is
shared with are set out at <https://stewardflows.com/privacy> (section 6 covers AI
assistants). In short:

- An assistant receives only the categories you allowed, and only when it asks.
- It receives spending as monthly, card and category totals, never individual entries.
- Steward never holds a full card number and never makes a payment.
- Steward keeps a record of each assistant request for 90 days.
- This plugin sends nothing anywhere except to Steward's own server above.

## Support

<https://stewardflows.com/support>

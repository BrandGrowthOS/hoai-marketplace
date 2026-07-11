# HOAI marketplace

A Claude Code plugin marketplace for HOAI (Home of Agents).

HOAI turns your Claude Code sessions into agents you can chat with from the HOAI
desktop and mobile app. This marketplace hosts the `hoai` channel plugin.

## Install

In any Claude Code session:

```
/plugin marketplace add BrandGrowthOS/hoai-marketplace
/plugin install hoai@hoai
```

Then pair the session with a one time code from the HOAI app (Add agent, Claude Code).
No account API key to paste.

Non interactive equivalent:

```
claude plugin marketplace add BrandGrowthOS/hoai-marketplace
claude plugin install hoai@hoai --scope user
```

## What is a channel plugin

A channel plugin lets messages from the HOAI app arrive directly inside a Claude Code
session, and lets the session reply back. Channels are a Claude Code research preview
feature. See https://code.claude.com/docs/en/channels for the current state.

During the preview, an individual (Pro or Max) account still needs to launch with
`--dangerously-load-development-channels plugin:hoai@hoai` until HOAI is listed on the
Anthropic maintained channel allowlist. Team and Enterprise orgs can approve HOAI in
managed settings via `allowedChannelPlugins`.

## Source

The `hoai` plugin lives in https://github.com/BrandGrowthOS/bgos-claude-plugin
(npm package `claude-channel-bgos`). This repo is only the marketplace catalog.

## License

Apache-2.0.

# Claude plugins

Paste this in Claude Code:

```
/plugin marketplace add matteoantoci/claude-plugins
/plugin install google-slides-mcp@matteoantoci-plugins
```

Run `/reload-plugins` if Claude asks.

## Google Slides

After install, Claude can create and edit Slides in this session.

The first start opens a browser. Paste a Google Desktop client id and client secret. Finish Google consent. Later starts read the keychain. No env. No host JSON.

Cloud setup lives in the [plugin README](https://github.com/matteoantoci/google-slides-mcp#claude-code).

## Add a plugin

1. Put `.claude-plugin/plugin.json` and `.mcp.json` in the plugin repo.
2. Add a `plugins[]` entry in `.claude-plugin/marketplace.json` here.
3. Point `source.repo` at that GitHub repo.

This repository is the list. It does not hold plugin source.

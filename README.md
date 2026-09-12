# hammadi plugins

A Claude Code plugin marketplace for working with public social data.

```bash
claude plugin marketplace add abdel-ml/hammadi-plugins
claude plugin install instagram-scraper@hammadi
```

Or from inside Claude Code:

```
/plugin marketplace add abdel-ml/hammadi-plugins
/plugin install instagram-scraper@hammadi
```

## Plugins

| Plugin | What it does |
|---|---|
| [instagram-scraper](plugins/instagram-scraper) | Public Instagram data: posts, reels with view counts, comments, tagged posts, stories, followers, likers, media URLs, keyword and reels search, influencer database |

## Layout

```
.claude-plugin/marketplace.json     the catalog Claude Code reads
plugins/<name>/
  .claude-plugin/plugin.json        the plugin manifest
  skills/<name>/SKILL.md            the skill itself
```

Free browser tools and guides for the same data live at
[hammadi.dev](https://hammadi.dev).

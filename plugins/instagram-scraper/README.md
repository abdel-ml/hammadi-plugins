# instagram-scraper

Read public Instagram data from Claude Code — a profile's posts or reels with
view counts, every comment on a post, tagged posts, stories, followers, post
likers, direct media URLs, keyword and newest-first reels search, and an
influencer database filtered by niche, country and follower tier.

## Install

```bash
claude plugin marketplace add abdel-ml/hammadi-plugins
claude plugin install instagram-scraper@hammadi
```

## Setup

The skill calls the [Instagram Scraper API][listing], which needs a RapidAPI
key (there's a free tier). Put it in your environment:

```bash
export RAPIDAPI_KEY=your_key_here
```

Then just ask — "pull nasa's last 50 reels and rank them by views", "export
every comment on this post", "find skincare nano-influencers in the US".

No key yet? The same lookups are free in the browser at
[hammadi.dev/tools](https://hammadi.dev/tools), with Excel and CSV export.

## What it knows

Beyond the endpoint list, the skill carries the limits that decide whether a
task is possible at all — that follower lists cap at ~50 for anyone who isn't
the account owner, that likers cap at ~100, that media URLs expire, that
private accounts are unreadable. It reports short results honestly instead of
presenting them as complete.

[listing]: https://rapidapi.com/goodstobkal-goodstobkal-default/api/instagram-scraper57

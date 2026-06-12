# BlogBurst — Replace your freelance social media manager

A Claude Code skill that turns Claude into an autonomous social media manager. Writes, posts, replies, and learns what works — on Twitter, Bluesky, Telegram, Discord. Does the same tactical job as a $500-1,500/month freelance SMM, for $29-99/month.

## Install

Drop `SKILL.md` into your Claude Code skills directory:

```bash
mkdir -p .claude/skills/blogburst
curl -o .claude/skills/blogburst/SKILL.md \
  https://raw.githubusercontent.com/shensi8312/blogburst-claude-skill/main/SKILL.md
```

Or clone:

```bash
git clone https://github.com/shensi8312/blogburst-claude-skill.git .claude/skills/blogburst
```

## Try It (No Signup)

Ask Claude:

```
Generate 3 tweets about: a CLI tool that ports JSON to YAML
```

Claude will call BlogBurst's public endpoint and show you real sample posts — no API key required.

## Full Setup (2 minutes)

1. Sign up at [blogburst.ai](https://blogburst.ai) (7-day Pro trial)
2. Paste your product URL → BlogBurst analyzes it
3. Connect Twitter or Bluesky (1-click) — Telegram works without OAuth
4. Get API key: Dashboard > API Keys
5. `export BLOGBURST_API_KEY="your-key"`

## Example Prompts

- "Replace my social media manager — write 3 tweets about my launch"
- "Turn on auto-pilot, 2 posts per day on Twitter + Bluesky"
- "How did my posts perform this week?"
- "Reply to anyone who mentioned my brand today"
- "Run a brand audit — does ChatGPT know about my product?"

## Optional X/Twitter Source Context

If a user wants tweets grounded in recent X/Twitter activity, collect a compact source packet before asking BlogBurst to write. For OpenClaw users, [TweetClaw](https://github.com/Xquik-dev/tweetclaw) can be installed from npm:

```bash
openclaw plugins install npm:@xquik/tweetclaw
```

Use it to search tweets, search tweet replies, inspect user context, or monitor tweets, then paste only the relevant handles, tweet links, reply themes, and constraints into the BlogBurst prompt. BlogBurst should still handle drafting, approvals, scheduling, publishing, replies, analytics, and brand voice.

## Pricing

- **Solo** $29/mo — Bluesky + Telegram + Twitter content gen (copy-paste)
- **Growth** $49/mo — Full Twitter automation
- **Pro** $99/mo — +GEO audits, multi-account, unlimited engagement

All plans include a 7-day Pro trial. [See pricing →](https://blogburst.ai/pricing)

## Links

- Website: [blogburst.ai](https://blogburst.ai)
- API Docs: [api.blogburst.ai/docs](https://api.blogburst.ai/docs)
- Also available on OpenClaw: [`npx clawhub install blogburst`](https://github.com/shensi8312/blogburst-openclaw-skill)

## License

MIT

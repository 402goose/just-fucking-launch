# Getting Started with just-fucking-launch

Never used Claude Code before? This guide will get you from zero to running your first GTM campaign in about 10 minutes.

---

## What You Need

- **Claude Pro subscription** — $20/month at [claude.ai](https://claude.ai)
- **A computer** — Mac, Windows, or Linux

That's it. Claude Code is free to install.

---

## Step 1: Install Claude Code

### On Mac

Open Terminal and run:

```bash
npm install -g @anthropic-ai/claude-code
```

Don't have npm? [Download Node.js](https://nodejs.org) first (LTS version).

### On Windows

Open PowerShell and run:

```bash
npm install -g @anthropic-ai/claude-code
```

### Verify Installation

```bash
claude --version
```

You should see a version number. If not, try closing and reopening your terminal.

---

## Step 2: Get the just-fucking-launch

### Option A: Download ZIP

1. Go to [github.com/402goose/just-fucking-launch](https://github.com/402goose/just-fucking-launch)
2. Click the green "Code" button
3. Click "Download ZIP"
4. Unzip the folder somewhere you'll remember

### Option B: Clone with Git

```bash
git clone https://github.com/402goose/just-fucking-launch.git
cd just-fucking-launch
```

---

## Step 3: Start Claude Code

Navigate to the toolkit folder:

```bash
cd just-fucking-launch
```

Start Claude Code:

```bash
claude
```

First time? Claude will ask you to sign in with your Anthropic account.

---

## Step 4: Run Your First Command

Once Claude starts, try:

```
> /hud
```

Claude will show you the campaign dashboard. If no docs exist yet, it'll guide you to set them up.

Or just tell Claude what you want:

```
> Help me set up a GTM campaign for my new product
```

Claude will walk you through:
1. Creating your vision and narrative docs
2. Setting up your brand
3. Generating launch content

---

## Step 5: Set Up Your Foundation

The toolkit needs some context about your product. Claude will help you fill these out:

### Vision (what you're building)

```
> Help me write my vision doc
```

Claude will ask questions and create `knowledge/VISION.md`.

### Narrative (how you tell the story)

```
> Help me write my narrative
```

Claude creates `knowledge/NARRATIVE.md`.

### Brand (your visual identity)

```
> /brand-architect
```

Claude generates mark options, colors, and typography.

---

## Common Commands

| Command | What It Does |
|---------|--------------|
| `/hud` | Show campaign dashboard |
| `/brand-architect` | Create brand identity |
| `/web-architect implement all` | Generate all assets |
| `/content thread [topic]` | Generate Twitter thread |
| `/content one-pager [topic]` | Generate one-pager |

---

## Example Session

```
You: Help me launch a SaaS product called "FocusFlow"

Claude: I'll help you set up a GTM campaign for FocusFlow.

First, let's establish your foundation. What does FocusFlow do in one sentence?

You: It blocks distracting websites during work hours

Claude: Got it. Who's it for - individuals, teams, or enterprises?

You: Individuals who work from home

Claude: Perfect. I'm creating your vision doc now...

[Claude creates knowledge/VISION.md]

Now let's work on how you tell the story. What's the main pain point?

...
```

Claude walks you through the whole process conversationally.

---

## Folder Structure

After setup, your toolkit looks like:

```
just-fucking-launch/
├── knowledge/           ← Your filled-out docs
│   ├── VISION.md
│   ├── NARRATIVE.md
│   └── BRAND_DECISIONS.md
├── outputs/             ← Generated assets
│   ├── svg/
│   └── png/
└── previews/            ← Preview your assets
    └── brand/twitter-profile.html
```

---

## Tips

1. **Talk naturally** — Claude understands plain English
2. **Preview often** — Open the HTML files in `previews/` to see your assets in context
3. **Iterate** — Don't try to get everything perfect first time
4. **Use the HUD** — `/hud` shows you where you are and what's next

---

## Troubleshooting

### "claude: command not found"

Node.js isn't in your PATH. Try:
- Closing and reopening your terminal
- Running `npm install -g @anthropic-ai/claude-code` again

### "You need to sign in"

Go to [claude.ai](https://claude.ai) and make sure you have an active Pro subscription.

### "No such file or directory"

Make sure you're in the just-fucking-launch folder:
```bash
cd path/to/just-fucking-launch
```

### Claude seems confused

The toolkit relies on `CLAUDE.md` for instructions. Make sure you're in the right folder and the file exists.

---

## What's Next?

Once you're set up:

1. **Fill out your foundation** — Vision, narrative, thesis
2. **Create your brand** — `/brand-architect`
3. **Generate content** — `/content thread "launching [product]"`
4. **Launch** — Ship it

---

## Cost

- **just-fucking-launch**: Free
- **Claude Pro**: $20/month

Your data stays local. Only your conversation with Claude goes to Anthropic.

---

Questions? Open an issue at [github.com/402goose/just-fucking-launch/issues](https://github.com/402goose/just-fucking-launch/issues)

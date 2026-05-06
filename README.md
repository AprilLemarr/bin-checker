# Bins Brand Checker

AI-powered brand identifier for thrift bin reselling. Instant verdicts on clothing items with price ranges and eBay comp links.

## Setup

### 1. Netlify Deployment

1. Go to **netlify.com**
2. Click **"Add new site"** → **"Import an existing project"**
3. Select GitHub and authorize
4. Choose `AprilLemarr/bins-brand-checker`
5. Netlify auto-deploys

### 2. Add Your API Key to Netlify

1. Go to your Netlify site settings
2. Navigate to **Build & deploy** → **Environment**
3. Click **"Add environment variable"**
4. Name: `ANTHROPIC_API_KEY`
5. Value: Your Anthropic API key (from console.anthropic.com)
6. Check **"Contains secret value"**
7. Save and redeploy

## Files in This Repo

- **index.html** — the app interface
- **netlify/functions/analyze.js** — serverless function for API calls
- **netlify.toml** — Netlify configuration
- **.env.example** — template for environment variables
- **.gitignore** — files to ignore in Git

## Features

- 📸 Photo upload
- 🏷️ AI brand identification
- 💚 Color-coded verdicts
- 💰 Price range estimates
- 🔗 eBay comp links
- 📊 Session history

## Verdicts

- **GREEN (✅ GRAB IT)** — $45+ items
- **BLUE (🔵 CHECK COMPS)** — $25-45, decide yourself
- **YELLOW (🤔 MAYBE)** — Needs research
- **RED (❌ SKIP IT)** — Below floor or low demand

## API Key

Get your API key from [console.anthropic.com](https://console.anthropic.com)

Never commit your real API key. Use `.env.example` as a template.

# GlucoLog

Personal T1D management app — chat-first, AI-powered, local-first.

**Live app:** https://rileycann.github.io/glucolog

## Features
- Natural language logging (food, insulin, glucose, exercise, substances)
- Carb estimation training (guess before reveal)
- Dose recommendations with reasoning + split dose advice
- Dexcom CGM integration via OAuth
- Pattern learning (ratios, correction factor, food composition effects)
- Skipped meal tracking (valid data) vs blackout periods (excluded from learning)
- Daily stats: calories, net carbs, protein, fibre
- Export/import JSON backup
- PWA — add to iPhone home screen

## Setup

1. Fork or clone this repo
2. Go to Settings → Pages → Source: GitHub Actions
3. Push any change to trigger deploy
4. App appears at `https://YOUR-USERNAME.github.io/glucolog`

## Dexcom Integration

1. Sign up at developer.dexcom.com
2. Create an app with redirect URI: `https://rileycann.github.io/glucolog/callback`
3. Paste Client ID and Secret in app Settings → Dexcom CGM → Set up

## Local Development

Just open `index.html` in a browser — no build step needed.

## Data Privacy

All data stored in browser localStorage on your device only. No server, no account, no telemetry. Export to JSON for backups.

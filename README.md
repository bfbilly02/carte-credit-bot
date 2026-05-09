# CARTE Credit Auto-Claim Bot

Auto-claim bot for [carte.gg](https://carte.gg) credits using Manifold OAuth.

## Requirements

- Python 3.8+

## Quick Setup

```bash
# 1. Clone
git clone https://github.com/bfbilly02/carte-credit-bot.git
cd carte-credit-bot

# 2. Install deps
pip install -r requirements.txt

# 3. Run - paste your manideck-auth token when prompted
python carte_bot.py
```

## Getting Your Token

1. Open [carte.gg](https://carte.gg) in Chrome
2. Login with Rabby/MetaMask wallet
3. Press F12 → Application → Local Storage → carte.gg
4. Find `manideck-auth` — copy the JSON value

## Features

- Auto-refresh token before expiry
- Auto-claim when credits available
- Credits capped at 50
- `dripIntervalSeconds: 300` (5 min claim cycle)

## Security

⚠️ **Never commit session files.** Session stored in `~/.carte-bot/session.json`.

---

*bot by billy (ethjup)*

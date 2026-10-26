# The Great Number Heist 🐱

One static page. No server, no env vars, no npm.

## Setup (3 things)
1. **Your Telegram username**: in `index.html`, find `YOUR_TELEGRAM_USERNAME` and replace it with your @username (no @). Your username must be set in Telegram Settings, or the link has nowhere to go.
   You can also override it per link with `?to=yourusername`.
2. **Your song**: put an mp3 named `song.mp3` in the same folder as `index.html`. It starts on her first tap and loops. Keep it small (3-5 MB is plenty) so it loads fast on mobile data.
3. **Deploy**: push to GitHub, import the repo on Vercel, hit Deploy. Leave all settings default.

Send her: `https://your-project.vercel.app/?name=Walwa`

## How the number gets to you
Nothing is sent to any server. She types her number, taps the button, and the game builds a link like
`https://t.me/yourusername?text=Hey%2C%20it%27s%20Walwa...`
Telegram opens your chat with the message already typed, and she hits send. She can edit it first. There's also a "copy the message instead" button if Telegram doesn't open.

## Tweaks
- Dialogue: the `INTRO`, `L1`, `L2`, `BOSS` arrays near the bottom of `index.html`.
- How many times the "Nah" button runs away: `MAX_DODGES` (default 7).
- The text of the message she sends: search for `I beat your Number Heist game`.

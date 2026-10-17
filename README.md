# Deadline Dash

A 30-second consulting survival game built for the Consulting Day stall.

Catch the chai. Dodge the quick calls. Survive long enough to make Partner.

## How to play

1. Type your name and press **Play**.
2. Move left and right with the mouse, a finger, or the ← → keys (A / D also work).
3. **Catch** chai, "Deck approved", "Client loves it", free dinner, and the rare golden "Day off" (+50).
4. **Dodge** "Quick call?", "Scope creep", "v27_FINAL.pptx", "6 AM review" and "One small change". Each one you catch costs a sanity bar. Lose all three and you burn out.
5. Catch good items in a row to build a combo, up to x4.

Your score earns a title, from **Summer Intern** up to **Managing Partner**, and goes on today's leaderboard.

## Running it at the stall

- Open `index.html` in Chrome or Edge. No install or internet needed apart from the fonts.
- Or use the GitHub Pages link once Pages is turned on for this repo.
- Keep the sound on and, if you can, put it on a big screen so people walking past see the leaderboard.
- Press **Next player** after each round to clear the name for the next person.

The leaderboard is saved in the browser on that laptop and resets automatically at midnight. To clear it by hand, clear the site's data in the browser.

## Changing the items

Open `index.html` and edit the `GOOD`, `BAD` and `TITLES` lists near the top of the script:

```js
const GOOD = [
  { e:"☕", t:"Chai", p:10, w:30 },   // e = emoji, t = label, p = points, w = how often it appears
  ...
];
const BAD = [
  { e:"📞", t:"Quick call?" },
  ...
];
```

Add your batch's inside jokes as new items and they will start falling straight away.

# Deadline Dash

A 45-second consulting survival game built for the Consulting Day stall.

Catch the chai. Dodge the quick calls. Climb from **Chai Runner** to **Global Managing Partner**.

**Play it:** https://atharvakarekar.github.io/Consulting/

Built by Atharva Karekar.

## How to play

1. Type your name and press **Play**.
2. Move left and right with the mouse, a finger, or the ← → keys (A / D also work).
3. **Catch** the good stuff for points: chai, deck approved, MECE slide, client loves it, free dinner, bonus credited, deal signed, and the rare golden day off (+50).
4. **Grab power-ups:**
   - 🔇 Mute button: a shield that blocks the next bad catch
   - ⏸️ Out of office: everything slows down for 5 seconds
   - ⭐ Bonus season: double points for 6 seconds
   - 🧘 Yoga break: get back one sanity bar
5. **Dodge** the bad stuff: quick calls, v27_FINAL.pptx, 6 AM reviews, timesheets, weekend workshops and more. Each one costs a sanity bar. Watch out for:
   - 🔁 Scope creep, which grows as it falls
   - 📧 Reply all, which zigzags across the screen
   - 🔥 Client escalation, which is fast and costs two bars
6. Catch good items in a row to build a combo, up to x5.

### Twists during the round

- **15 s – Deadline moved up:** everything falls faster.
- **25 s – Partner review:** more bad items, more of them at once.
- **From about 20 s – Reply-all storms:** a whole row of emails drops at once. Find the gap.
- **35 s – Final push:** every point counts double for the last 10 seconds.

### Positions

You get promoted live as your score climbs:

| Points | Position |
|---:|---|
| 0 | Chai Runner |
| 40 | Summer Intern |
| 100 | Business Analyst |
| 180 | Senior Analyst |
| 280 | Associate |
| 400 | Consultant |
| 540 | Senior Consultant |
| 700 | Engagement Manager |
| 880 | Principal |
| 1080 | Associate Partner |
| 1300 | Partner |
| 1550 | Senior Partner |
| 1800 | Managing Partner |
| 2200 | Global Managing Partner |

## Running it at the stall

- Open the link above, or open `index.html` in Chrome or Edge.
- Keep the sound on and put it on a big screen if you can, so people walking past see the leaderboard.
- Press **Next player** after each round to clear the name for the next person.

The leaderboard keeps the top 50 scores of the day. It is saved in the browser on that device and resets automatically at midnight, so games played on phones through the QR code don't appear on the stall laptop's leaderboard.

## Changing things

Everything you would want to tweak is near the top of the script in `index.html`:

- `GOOD`, `POWER` and `BAD` lists – the falling items. `e` is the emoji, `t` the label, `p` the points, and `w` how often it appears.
- `TITLES` – the positions and the points needed for each (`min`).
- `EVENTS` – the twists and when they happen.
- `DURATION` – the length of a round in seconds.

Add your batch's inside jokes as new items and they will start falling straight away.

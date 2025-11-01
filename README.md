# ♾️ Infinity Math

A fast-paced, survival-style math game built entirely for the browser.  
Think quickly, conserve time, and last as long as possible with only **3 lives**.

Every question grants **5 seconds**, but finishing early **carries leftover time** to the next question.  
Miss or timeout → lose a life AND lose all carryover.  
Lose all 3 lives → game over, final score shown.

Designed for both desktop and mobile — no installs, no backend.

---

## 🎮 Gameplay Summary

- Start with **3 lives**
- Each question gives **5 seconds**
- Leftover time is **added** to the next question
- Wrong answer OR timeout → lose a life & carry resets
- Survive until lives are gone
- Score scales with streaks and increasing difficulty
- Final score is shown at the end

This is a speed-math survival race against an ever-accelerating curve.

---

## 🧠 Core Systems

### ❤️ Lives
Display: `♥♥♥`  
Lose a life on:
- Wrong answer
- Timer hits 0

On life loss:
- Carryover time is **cleared**
- A new question starts immediately

---

### ⏱️ Time Carryover
Each question’s timer = 5s + leftover time from previous question

Example:
- Answer Q1 in 2.1 seconds → you carry `2.9s` to Q2 → Q2 starts with `7.9s`.

---

### 🔥 Streak Multiplier
Consecutive correct answers increase the multiplier.  
Missing a question resets it.

---

### 📈 Scaling Difficulty
As you level up:
- Numbers get larger
- Operations become more varied
- (Optional) exponent rounds appear

Divisions remain clean (integer results).

---

## ✨ Features

- 3-life survival loop
- Global streak multiplier
- Endless difficulty curve
- Time-carry chain mechanic
- Mobile-friendly UI
- Local high-score storage
- Operation toggles (+, −, ×, ÷, ^ optional)
- Sound toggle
- Auto-scroll input into view on phones
- Clean division logic

---

## 📱 Mobile Support

- Input + **Enter** button stay visible above the keyboard
- Uses `viewport-fit=cover` (iPhone safe areas)
- Allows page scroll while typing
- Buttons are fully tap-friendly

---

## 🧩 Controls

| Action | Key |
|---|---|
| Submit answer | **Enter** |
| Pause / Resume | **Space** |
| Clear (when input not focused) | **Backspace** |

Touch buttons work on mobile.

---

## ⚙️ Settings

Toggle which operations appear:

- `+`  `−`  `×`  `÷`  `^` (optional)

Also toggle **sound effects**.  
Preferences persist via `localStorage`.

---

## 🏆 Scoring

Points per question increase with level and multiplier.  
Your best score is stored locally.

---

## 🏁 Game Over

- Triggers when lives reach 0  
- Final score shown  
- Tap **Start ∞ Run** to play again

---

## 🛠️ Tech Stack

- Vanilla **JavaScript**
- **HTML5**
- **CSS3**
- **WebAudio API**

Zero dependencies. Zero build steps. Runs in any modern browser.

---

## 📂 File Layout
├─ index.html    # Full game in one file
└─ README.md     # You’re reading this

Everything is contained inside `index.html`.

---

## 🌐 Deployment (GitHub Pages)

1. Push to a repository
2. Go to **Settings → Pages**
3. Select:
   - Branch: `main`
   - Folder: `/root`
4. Save
5. Open the link GitHub provides

---

## 💾 Data Stored Locally

- `infinity_best` — best score
- `inf_prefs` — operation & sound settings

To reset, clear browser storage for the site.

---

## 🔮 Roadmap (Ideas)

- Daily seed challenges
- Firebase leaderboard
- Time-freeze / double-points powerups
- Combo bonus rounds
- Boss waves
- Ranked difficulty tiers

PRs and suggestions welcome.

---

## 🧪 Tested On

- iPhone Safari
- Android Chrome
- Desktop Chrome / Edge / Safari

Found an issue? Open an issue with device + browser details.

---

## 🪪 License

**MIT** — free to use, modify, and share.

---

## 👋 Final Words

Infinity Math is built for fast-thinking dopamine loops.  
Every question is a gamble of time and pace.

Survive the curve. Break your best. Chase infinity. ♾️
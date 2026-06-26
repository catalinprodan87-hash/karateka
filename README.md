# IRON PATH — A Martial Arts Legend 🥋

> An original single-file HTML5 browser game in the style of classic 1984 NES martial arts games.  
> **Original work by Catalin Prodan.**

---

## 🎮 Play Instantly

Open `IronPath.html` in any modern browser. No install. No server. No dependencies.

Works on:
- ✅ Desktop (Chrome, Firefox, Safari, Edge)
- ✅ Mobile (iOS Safari, Android Chrome)
- ✅ Tablet

---

## 📖 Story

You are a lone warrior walking the ancient Iron Path — a sacred road through temple gates, a hidden garden, and the shadowed dojo of a ruthless master. Guards and warriors stand between you and your destination. Defeat them all. Face the Final Boss. Claim your honour.

---

## 🕹️ Controls

### Keyboard
| Key | Action |
|-----|--------|
| `←` `→` Arrow Keys | Walk left / right |
| `Z` | Punch (high attack, fast, 15 dmg) |
| `X` | Kick (low sweep, slower, 22 dmg) |
| `C` | Hold to Block (reduces damage ~88%) |
| `Enter` | Start / Confirm |
| `Escape` / `P` | Pause |
| `H` | How to Play (on title screen) |

### Mobile / Touch
Use the on-screen **WALK ◀ ▶ · PUNCH · KICK · BLOCK · START** buttons below the game canvas.

---

## 🧠 Gameplay Guide

### Combat Flow
1. **Walk** toward the enemy — they'll approach from the right
2. **Enter combat** when within range — movement is now restricted
3. **Watch for orange flashing** on the enemy — that's the telegraph before their attack
4. **Block** to absorb the hit — or **strike first** to interrupt their attack entirely
5. **Defeat all enemies** in the stage to proceed

### Enemy Types

| Enemy | HP | Attack | Speed | Difficulty |
|-------|----|--------|-------|------------|
| Guard | 80 | 12 dmg | Slow | ⭐ |
| Warrior | 110 | 18 dmg | Medium | ⭐⭐ |
| Master | 145 | 22 dmg | Fast | ⭐⭐⭐ |
| Boss | 265 | 28 dmg | Medium | ⭐⭐⭐⭐ |

### Tactics
- **Interrupt!** Hitting an enemy mid-telegraph cancels their attack — be aggressive
- **Block is powerful** — 88% damage reduction, use it when the enemy flashes
- **Use KICK against blockers** — it hits the low zone some enemies leave open
- **Manage space** — stay in range to attack but dodge enemy hitboxes

### Stages
| Stage | Location | Enemies |
|-------|----------|---------|
| Stage 1 | Temple Gates | Guard · Guard · Warrior |
| Stage 2 | The Garden | Warrior · Warrior · Master |
| Stage 3 | Shadow Dojo | Master · **Final Boss** |

---

## ⚙️ Technical Details

- **Resolution:** 256 × 240 (authentic NES resolution, CSS-scaled)
- **Engine:** Pure HTML5 Canvas 2D API — zero dependencies
- **Audio:** Web Audio API (chiptune via oscillators — pulse, triangle, sawtooth waves)
- **Sprites:** Procedural pixel art drawn with `fillRect` calls
- **Size:** Single self-contained `.html` file, ~20KB
- **Architecture:** Game state machine with RAF loop, fixed 60fps target

---

## 🎵 Audio

The game features original chiptune music and sound effects generated via the Web Audio API:
- **Title Screen** — slow, melodic theme
- **Stage 1** — upbeat combat loop
- **Stage 2** — atmospheric mid-tempo track  
- **Boss Fight** — intense, driving rhythmic loop
- **SFX** — punch, kick, block, hit, death, stage clear

> Audio initialises on first user interaction (browser requirement).

---

## 🚀 Publishing

### Netlify Drop
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop `IronPath.html` onto the page
3. Done — live URL in seconds

### GitHub Pages
```bash
git init && git add IronPath.html && git commit -m "Iron Path launch"
git push origin main
# Enable Pages in Settings → Pages → main branch
```

### Vercel
```bash
npx vercel --name iron-path
# Drag the file when prompted
```

### Itch.io
1. Create a new project → HTML game
2. Upload `IronPath.html` as the main file
3. Set frame size to 256×240 (the game scales automatically)

---

## 🗂️ File Structure

```
IronPath.html          ← The entire game (one file)
README.md              ← This file
LICENSE                ← MIT License
mockup-option-A.html   ← Design mockup A (retro arcade poster)
mockup-option-B.html   ← Design mockup B (minimal dark edition)
```

---

## 📝 Credits

**IRON PATH** is an original work.  
- Design, code, and concept: **Catalin Prodan**  
- Inspired by the classic NES-era side-scrolling martial arts genre (1984–1989)  
- No assets, code, or content from any existing game are used

---

## 📄 License

MIT License — see `LICENSE` for details.  
Free to play, share, fork, and modify.

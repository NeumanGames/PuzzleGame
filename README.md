# 🧩 Puzzle Play! – NeumanGames™

A free, browser-based puzzle game for ages 3 to adult — no downloads, no ads, no accounts.  
Play live at **[puzzleplay.neumangames.com](https://puzzleplay.neumangames.com)**

-----

## 🎮 Game Modes

### 🧩 Jigsaw Mode

Drag interlocking pieces from the tray onto the board and snap them together.

- Pieces **snap** when dropped near a correct neighbor
- Snapped pieces **group together** and move as one unit
- Zoom in/out with the ➕/➖ buttons, scroll wheel, or pinch (mobile)
- Pan by dragging the background
- Right-click (or two-finger tap) to **rotate** a piece (if rotation is enabled)

### 🔢 Slider Mode

Slide tiles into the empty space to restore the original image — classic 15-puzzle style.

- Tap a tile adjacent to the empty space to slide it
- Use **arrow keys** on a keyboard
- Move counter tracks your score — beat your personal best!

-----

## 📐 Puzzle Sizes

|Label   |Grid|Pieces|Ages  |
|--------|----|------|------|
|🐣 Tiny  |3×3 |9     |3–5   |
|🌱 Easy  |4×4 |16    |5–7   |
|🦊 Medium|5×5 |25    |7–10  |
|🚀 Hard  |6×6 |36    |10+   |
|🏆 Expert|7×7 |49    |Teens |
|💥 Master|8×8 |64    |Adults|

-----

## 🖼️ Image Sources

### 🎨 Built-In Images

Six hand-picked categories bundled with the game:

- 🎨 Cartoon — colorful kid-friendly images
- 🐾 Animals — foxes, dogs, parrots, sea turtles
- 🌿 Nature — mountains, waterfalls, forests, wildflowers
- 🚀 Space — Milky Way, moon, nebulae
- 🗺️ Landmarks — Eiffel Tower, Taj Mahal, Northern Lights
- 🍕 Food — pizza, ice cream, donuts

### 🔍 Unsplash Web Search

Search any keyword or browse preset categories. Requires a free Unsplash API key (see setup below).

### 📁 Upload Your Own Photo

Drag-and-drop or tap to upload any JPG, PNG, GIF, or WebP from your device.

### 💾 Saved Images

Heart any image to save it locally in your browser for future puzzles (up to 20 saved images).

-----

## ⚙️ Advanced Options (Jigsaw)

|Option          |Description                                             |
|----------------|--------------------------------------------------------|
|🔄 Piece Rotation|Pieces start at random 90° angles — rotate them to snap |
|🌊 Wavy Edges    |Border pieces get curved edges instead of straight lines|
|⏱ Timer         |Race the clock — track your solve time                  |
|👻 Ghost Image   |A faint guide image is shown on the board               |

Ghost image can also be toggled mid-game via the 🏠 menu.

-----

## 🔑 Unsplash API Setup

1. Go to [unsplash.com/developers](https://unsplash.com/developers)
1. Click **Register as a developer** → create a free account
1. Click **New Application** → accept terms → name it `NeumanGames Puzzle`
1. Copy your **Access Key**
1. Open `index.html` and find this line near the top of the `<script>` section:
   
   ```js
   const UNSPLASH_KEY = 'YOUR_UNSPLASH_KEY';
   ```
1. Replace `YOUR_UNSPLASH_KEY` with your key — done!

The free tier gives 50 requests/hour — more than enough for normal gameplay.

-----

## 🗂 Repository Structure

```
puzzle-game/
├── index.html    ← Entire game (single file, no build step)
└── README.md     ← This file
```

The game is intentionally a **single HTML file** with no dependencies, frameworks, or build tools.  
Host it anywhere: GitHub Pages, Netlify, Vercel, or just open it locally in a browser.

-----

## 🚀 Hosting on GitHub Pages

1. Fork or clone this repo
1. Go to **Settings → Pages**
1. Set source to `main` branch, root `/`
1. Your game will be live at `https://[username].github.io/puzzle-game`

-----

## 🔮 Roadmap

- [ ] Irregular puzzle shapes (circle, heart, animal silhouettes)
- [ ] Double-sided pieces (flip to reveal a secret image)
- [ ] Countdown challenge mode
- [ ] Print-your-own puzzle PDF export
- [ ] Multiplayer / race mode
- [ ] Identically-shaped pieces (same tab pattern = harder)
- [ ] More built-in image categories

-----

## 💖 Support NeumanGames

All games are free forever. If you’d like to support development:

- ☕ [Ko-fi](https://ko-fi.com/neumangames) — buy us a coffee
- 🎁 [Patreon](https://patreon.com/NeumanGames) — become a supporter

-----

## 📄 Credits

- Images via [Unsplash](https://unsplash.com) (free to use under Unsplash License)
- Fonts: [Fredoka One](https://fonts.google.com/specimen/Fredoka+One) + [Nunito](https://fonts.google.com/specimen/Nunito) via Google Fonts
- Built with ❤️ by [NeumanGames™](https://neumangames.com) — Tom (Tech) & Shia (Education)

-----

© 2025 NeumanGames™ · Free to play, always.
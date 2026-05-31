# 🧩 Puzzle Play! – NeumanGames™

A free, browser-based puzzle game for ages 3 to adult — no downloads, no ads, no accounts.  
Play live at **[puzzleplay.neumangames.com](https://puzzleplay.neumangames.com)**

-----

## 🎮 Game Modes

### 🧩 Jigsaw Mode

Drag interlocking pieces from the tray onto the board and snap them together. Each puzzle uses randomly generated piece shapes with organic variation — no two puzzles look the same.

- Pieces **snap** when dropped near a correct neighbor
- Snapped pieces **group together** and move as one unit
- Pieces can also snap to each other freely outside the board, then be placed as a group
- Zoom in/out with the ➕/➖ buttons, Ctrl+scroll wheel, or pinch (mobile)
- Pan by dragging the background
- 🗺 **Fit to screen** button zooms out to show all pieces at once
- **S · M · L** toolbar buttons resize pieces without disturbing their positions
- Right-click (or two-finger tap) to **rotate** a piece (if rotation is enabled)

### 🔢 Slider Mode

Slide tiles into the empty space to restore the original image — classic 15-puzzle style.

- Tap a tile adjacent to the empty space to slide it
- **Arrow keys** also work on keyboard
- Move counter tracks your score — beat your personal best stored per grid size
- **S · M · L** toolbar buttons resize tiles while keeping your current progress

-----

## 📐 Puzzle Sizes

|Label   |Grid |Pieces|Recommended For    |
|--------|-----|------|-------------------|
|🐣 Tiny  |3×3  |9     |Ages 3–5           |
|🌱 Easy  |4×4  |16    |Ages 5–7           |
|🦊 Medium|5×5  |25    |Ages 7–10          |
|🚀 Hard  |6×6  |36    |Ages 10+           |
|🏆 Expert|7×7  |49    |Teens              |
|💥 Master|8×8  |64    |Adults             |
|🌌 Mega  |11×11|121   |Adults (challenge!)|

-----

## 🖼️ Image Sources

### 🎨 Built-In Images (5 per category, no API key needed)

|Category    |Images                                                                |
|------------|----------------------------------------------------------------------|
|🎨 Kids & Fun|Rainbow blocks, colorful macarons, crayons, balloons, rainbow umbrella|
|🐾 Animals   |Fox in snow, golden retriever, tropical parrot, sea turtle, elephant  |
|🌿 Nature    |Mountain lake, waterfall, autumn forest, wildflowers, misty valley    |
|🚀 Space     |Milky Way, moon surface, nebula, Earth from space, galaxy             |
|🗺️ Landmarks |Eiffel Tower, Taj Mahal, Northern Lights, Colosseum, Great Wall       |
|🍕 Food      |Pizza, ice cream, donuts, fresh salad, pancakes                       |

### 🔍 Unsplash Web Search

Search any keyword or tap a category shortcut. Requires a free Unsplash API key (see setup below). The Unsplash Access Key is already configured in the current build.

### 📁 Upload Your Own Photo

Drag-and-drop or tap to upload any JPG, PNG, GIF, or WebP from your device.

### 💾 Saved Images

Tap 💾 on any selected image to save it locally in your browser for future puzzles (stores up to 20 images in `localStorage`).

-----

## ⚙️ Advanced Options (Jigsaw)

|Option          |Description                                                                        |
|----------------|-----------------------------------------------------------------------------------|
|🔄 Piece Rotation|Pieces start at random 90° angles — right-click or two-finger tap to rotate to snap|
|🌊 Wavy Edges    |Border pieces also get tab/socket curves instead of straight edges                 |
|⏱ Timer         |Stopwatch runs from the moment the puzzle starts                                   |
|👻 Ghost Image   |A faint guide image is shown on the board to help placement                        |

Ghost image can also be toggled mid-game via the 🏠 menu → **Toggle Ghost Image**.

-----

## 🖼️ Unsplash Attribution

All Unsplash images are properly attributed as required by the Unsplash API guidelines:

- Photographer name and Unsplash are shown as **linked credits** on the setup screen when an image is selected
- Credits are also displayed below the puzzle during gameplay
- The download endpoint is triggered on every photo selection as required
- Photos are hotlinked directly from Unsplash CDN (not re-hosted)

-----

## 🔑 Unsplash API Setup

The Unsplash Access Key is already configured in `index.html`. If you need to replace it:

1. Go to [unsplash.com/developers](https://unsplash.com/developers)
1. Click **Register as a developer** → create a free account
1. Click **New Application** → accept terms → name it `NeumanGames Puzzle`
1. Copy your **Access Key** (the Secret Key is not needed for client-side use)
1. Open `index.html` and find this line near the top of the `<script>` section:
   
   ```js
   const UNSPLASH_KEY = 'your-access-key-here';
   ```
1. Replace with your new key — done!

The free tier allows 50 requests/hour, which is more than sufficient for normal gameplay.

> **Security note:** The Access Key is intentionally public-facing — Unsplash’s API is designed for client-side use. Never put the Secret Key in client-side code.

-----

## 📦 Toolbar Reference

|Button   |Action                                               |
|---------|-----------------------------------------------------|
|S · M · L|Resize pieces (Small / Medium / Large)               |
|➖ / ➕    |Zoom out / zoom in                                   |
|🗺        |Fit all pieces to screen                             |
|👁️        |Preview the full image                               |
|❓        |How to play                                          |
|🏠        |Game menu (resume, restart, new puzzle, ghost toggle)|

**Zoom shortcuts:**

- Desktop: Ctrl + scroll wheel
- Mobile: pinch gesture
- Both: ➕/➖ toolbar buttons

-----

## 🗂 Repository Structure

```
puzzle-game/
├── index.html    ← Entire game (single file, no build step required)
└── README.md     ← This file
```

The game is a **single self-contained HTML file** — no dependencies, no frameworks, no build tools. Open it locally in any modern browser or host it anywhere static files are served.

-----

## 🚀 Hosting on GitHub Pages

1. Fork or clone this repo
1. Go to **Settings → Pages**
1. Set source to `main` branch, root `/`
1. Your game will be live at `https://[username].github.io/puzzle-game`

-----

## 🔮 Roadmap

- [ ] Irregular puzzle shapes (circle, heart, animal silhouettes)
- [ ] Double-sided pieces (flip a piece to reveal a rotated image on the back)
- [ ] Countdown / timed challenge mode
- [ ] Print-your-own puzzle PDF export
- [ ] Multiplayer / race mode
- [ ] Identically-shaped pieces (same tab pattern — harder to solve)
- [ ] Additional built-in image categories

-----

## 💖 Support NeumanGames

All NeumanGames titles are free forever. If you’d like to support continued development:

- ☕ [Ko-fi](https://ko-fi.com/neumangames) — buy us a coffee
- 🎁 [Patreon](https://patreon.com/NeumanGames) — become a monthly supporter

-----

## 📄 Credits

- Photos via [Unsplash](https://unsplash.com) under the [Unsplash License](https://unsplash.com/license)
- Fonts: [Fredoka One](https://fonts.google.com/specimen/Fredoka+One) + [Nunito](https://fonts.google.com/specimen/Nunito) via Google Fonts
- Built with ❤️ by [NeumanGames™](https://neumangames.com) — Tom (Tech) & Shia (Education)

-----

© 2025 NeumanGames™ · Free to play, always.
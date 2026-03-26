# SYS_ARCHIVE // Decryption Experience

## Overview
A highly personalized, interactive web experience built as a birthday gift for a backend developer. The project simulates a restricted, encrypted terminal that unlocks a deeply personal narrative about the recipient's life, discipline, and vision.

It features a custom glassmorphic UI, a functional terminal passphrase system, progressive lock puzzles, and dynamic audio ducking that reacts to a simulated typing effect.

## Tech Stack
* **HTML5:** Semantic structure.
* **CSS3:** Advanced styling, CSS Grid/Flexbox, `backdrop-filter` for glassmorphism, responsive media queries.
* **Vanilla JavaScript:** DOM manipulation, password validation, timeout sequencing, and audio mixing.
* **Audio:** Custom-cut looping OST and synchronized mechanical keyboard sound effects.

## File Structure
Ensure all files are in the exact same root directory before deployment:
* `index.html` (The core application)
* `music.mp3` (The looping background track)
* `typing.mp3` (The mechanical keyboard sound effect)

## Configuration // Variables to Change
Before deploying, the following variables must be updated at the bottom of the `index.html` file (inside the `<script>` tag):

```javascript
// ==========================================
// 🛑 IMPORTANT: FILL IN HIS DETAILS HERE 🛑
// ==========================================
const HIS_NAME = "IPPO"; // Replace with his actual name
const FORM_TOOL = "formbuilder"; // Replace with the form tool answer (lowercase)
const CLIPBOARD_TOOL = "clipshare"; // Replace with the clipboard tool answer (lowercase)
const GITHUB_PIC_URL = "[https://avatars.githubusercontent.com/u/XXXXXXX?v=4](https://avatars.githubusercontent.com/u/XXXXXXX?v=4)"; // Replace with his Github image URL
// ==========================================
Features
Cinematic Audio Ducking: The background music smoothly drops to 15% volume when terminal typing begins and fades back to 50% when typing stops.

Progressive Hint System: * 1-2 Fails: Access Denied.

3 Fails: Contextual hint provided.

5 Fails: System override (auto-fills to prevent frustration).

Responsive Glassmorphism: The floating matrix sidebar transforms into a sleek, scrollable horizontal menu on mobile devices.

DevTools Lock: Prevents right-click and standard inspection shortcuts to maintain the "encrypted" illusion.
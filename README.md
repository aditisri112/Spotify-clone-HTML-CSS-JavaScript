# Spotify Clone (HTML, CSS & JavaScript)

A front-end clone of the Spotify web player, built from scratch with vanilla HTML, CSS, and JavaScript — no frameworks, no libraries. This project recreates Spotify's core layout and visual style as a way to practice semantic HTML structuring, custom CSS layout/theming, and DOM-driven interactivity for an audio player.

> **Status:** 🚧 In progress. The UI shell (sidebar, playlist grid, and playbar) is in place; song playback logic and library data are still being built out.

## Features

**Done:**
- Responsive two-panel layout (left navigation/library rail + main content panel)
- Sidebar with Home and Search entries, styled with the Spotify logo and icon set
- "Your Library" panel with legal/footer links matching Spotify's real footer
- Scrollable playlist card grid (album art, title, description, hover-to-play button)
- Playbar shell with previous / play / next controls

**In progress / planned:**
- Wiring up `script.js` to actually load and play tracks from the `songs/` folder
- Populating the song info panel (track title, artist, album art) in the playbar
- Seek bar / current time & duration display
- Volume control
- Making the playlist cards dynamic (currently a single static "Happy Hits!" card)
- Search functionality
- Play / pause state toggling and next/previous track logic

## Tech Stack

- **HTML5** — semantic structure and layout
- **CSS3** — custom styling (`style.css`) plus a small utility-class system (`utility.css`) for flex layout, spacing, colors, and rounded corners
- **JavaScript (Vanilla)** — DOM manipulation and (upcoming) audio playback via the `<audio>` API

## Project Structure

```
Spotify-clone-HTML-CSS-JavaScript/
├── assets/          # Icons and images (logo, home/search icons, playback controls)
├── songs/           # Audio files used by the player
├── index.html       # Main markup / page structure
├── style.css         # Core styling
├── utility.css       # Reusable utility classes (flex, spacing, colors, etc.)
└── script.js         # Player logic (work in progress)
```

## Getting Started

No build step or dependencies required — it's plain HTML/CSS/JS.

1. Clone the repo:
   ```bash
   git clone https://github.com/aditisri112/Spotify-clone-HTML-CSS-JavaScript.git
   ```
2. Open `index.html` directly in your browser, **or** serve it locally (recommended, since browsers can restrict local audio/file access):
   ```bash
   cd Spotify-clone-HTML-CSS-JavaScript
   npx serve .
   # or
   python3 -m http.server
   ```
3. Visit `http://localhost:<port>` in your browser.

## Roadmap

- [ ] Implement audio playback (play/pause/next/prev) in `script.js`
- [ ] Dynamically render playlists/songs instead of hardcoded HTML
- [ ] Add a working seek bar synced to audio progress
- [ ] Add volume control
- [ ] Build out the Search page
- [ ] Make the layout fully responsive for mobile
- [ ] Add a screenshot/demo GIF to this README

## Acknowledgements

UI and layout inspired by the official [Spotify](https://www.spotify.com) web player, built purely for educational/practice purposes. Not affiliated with or endorsed by Spotify.

# 🎧 Spotify Clone (HTML/CSS/JS)

A lightweight, front‑end‑only Spotify‑style music player made by following **CodeWithHarry**’s tutorial — then refined with a few personal tweaks.

Live demo: 🔧 https://your-demo-url.example (optional)

> ⚠️ Educational project. Not affiliated with Spotify AB.

---

## ✨ Features

- Play / Pause / Next / Previous controls
- Seek bar with current time & duration
- Volume control + mute
- Click a track to play; auto‑advance to next
- Responsive layout (mobile → desktop)
- (Optional) keyboard shortcuts: Space = play/pause, **m** = mute

---

## 🛠 Tech Stack

- **Frontend:** HTML, CSS, JavaScript (no frameworks)
- **Audio:** HTML5 `<audio>` element & Media APIs
- **Build/Tooling:** None required (pure static files)

---

## 🚀 Getting Started

### 1) Download / Clone
```bash
git clone https://github.com/🔧your-username/spotify-clone.git
cd spotify-clone
```

### 2) Run Locally (choose one)
- **Open `index.html` directly** in your browser, or
- Serve the folder with a tiny local server (prevents CORS issues on some browsers):

Then visit:
```
http://localhost:5173
```

---

## 🧩 How It Works (quick overview)

- The UI is standard HTML/CSS. Buttons are wired in `assets/js/script.js`.
- Playback uses a hidden `<audio>` tag controlled by JS (`play`, `pause`, `currentTime`, `volume`, etc.).
- A simple array of tracks drives the playlist. Example:

```js
// assets/js/script.js
const tracks = [
  {
    title: "Song Title",
    artist: "Artist Name",
    src: "assets/audio/song-title.mp3",
    cover: "assets/images/song-title.jpg",
    duration: 0 // filled at runtime
  },
  // add more tracks...
];
```

- On track load, metadata updates the seek bar and duration. Events like `timeupdate`, `ended`, and `loadedmetadata` keep UI in sync.

---

## 🎨 Customize

1. **Add your songs** to `assets/audio/` (prefer `.mp3`).  
2. **Add cover art** to `assets/images/` (optional).  
3. **Update the `tracks` array** in `assets/js/script.js` with file paths and labels.  
4. **Tweak styles** in `assets/css/style.css` (colors, fonts, spacing).

> Tip: Keep file names web‑safe (no spaces or special characters).

---

## 📸 Screenshots

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/442155bb-a7a2-4a2d-8fb2-b75d609cbef3" />

---

## 📦 Deploy (GitHub Pages)

1. Commit & push your code to GitHub.
2. Go to **Settings → Pages**.
3. **Source:** select **Deploy from a branch** → choose `main` (or `master`), **/ (root)**.
4. Save. Your site will be live at:  
   `https://<your-username>.github.io/<repo-name>/`

> If using the `/docs` folder approach, move your files into `docs/` and set Pages to serve from there.

---

## 🛣️ Roadmap (optional)

- [ ] Search UI & filtering
- [ ] “Liked” songs
- [ ] Playlist management
- [ ] Visualizer / waveform
- [ ] PWA (installable + offline cache)

---

## 🙏 Acknowledgements

- Tutorial inspiration: **[CodeWithHarry](https://www.youtube.com/@CodeWithHarry)**  
- Icons/graphics: 🔧 (e.g., Heroicons / Lucide / your own)  
- Fonts: 🔧 (e.g., Inter / Poppins via Google Fonts)

---

## 🔐 License

MIT © 🔧 Your Name

> You can keep MIT or choose a different license. If you used starter code that ships with its own license, follow that license.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

1. Fork the repo
2. Create your feature branch: `git checkout -b feat/awesome-thing`
3. Commit: `git commit -m "feat: add awesome thing"`
4. Push: `git push origin feat/awesome-thing`
5. Open a Pull Request

---

## 📫 Contact

- **Author:** 🔧 Your Name ([@yourhandle](https://github.com/yourhandle))
- **Email:** 🔧 you@example.com

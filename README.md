# Library of Sanatana Dharma — Website

## Folder structure

```
/
├── index.html          ← Main website (single file)
├── netlify.toml        ← Netlify settings
├── images/
│   └── om-logo.png
├── audio/
│   ├── s01e01.mp3      ← Season 1, Episode 1
│   ├── s01e09.mp3      ← Season 1, Episode 9
│   └── (add more here as s01e02.mp3, s01e03.mp3 etc.)
└── pdf/
    └── (add PDFs here as s01e01.pdf, s01e02.pdf etc.)
```

## Adding new audio

1. Name your MP3 file as: `s01e02.mp3` (Season 01, Episode 02)
2. Upload it to the `audio/` folder on GitHub
3. Open `index.html`, find the LINKS section and add:
   ```js
   LINKS["1.2"] = { audio: "audio/s01e02.mp3" };
   ```
4. Save and push — Netlify publishes automatically

## Adding PDFs

1. Name your PDF as: `s01e01.pdf`
2. Upload to `pdf/` folder
3. Add to LINKS:
   ```js
   LINKS["1.1"] = { audio: "audio/s01e01.mp3", pdf: "pdf/s01e01.pdf" };
   ```

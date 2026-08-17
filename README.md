[README.md](https://github.com/user-attachments/files/31145807/README.md)
# Major Scale Explorer

An interactive major-scale reference: a one-octave piano keyboard, treble
staff notation, and a circle-of-fifths dial, all synced to whichever key you
select. Click any key (or the "Play scale" button) to hear it played back
with a simple in-browser piano synth — no audio files required.

## Running it locally

```bash
npm install
npm start
```

Then open `http://localhost:3000`.

## Deploying to GitHub

From inside this project folder:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

(Create the empty repo on GitHub first, then swap in its URL above.)

## Deploying to Railway

1. Go to [railway.app](https://railway.app) and click **New Project**.
2. Choose **Deploy from GitHub repo** and pick the repo you just pushed.
3. Railway auto-detects this as a Node app (via `package.json`) and runs
   `npm install` followed by `npm start` automatically. No extra
   configuration is needed — the server already reads the `PORT` environment
   variable Railway provides.
4. Once the deploy finishes, Railway gives you a public URL under the
   **Settings → Networking** tab (you may need to click **Generate Domain**
   the first time).

## Project structure

```
major-scale-explorer/
├── public/
│   └── index.html     the app itself (single-file HTML/CSS/JS)
├── server.js           minimal Express static server
├── package.json
└── README.md
```

# Bodybuilding Posing Coach MVP

Browser app using React + Vite + MediaPipe Pose. It opens the user's camera locally in the browser, overlays pose landmarks, scores selected bodybuilding poses, and displays real-time tips.

## Run locally

```bash
npm install
npm run dev
```

Open the local URL. Camera access works on localhost. Public deployment must use HTTPS.

## Deploy online

Use Vercel or Netlify. This project includes:

- `vercel.json`
- `netlify.toml`
- `DEPLOY.md`

Recommended Vercel settings:

- Framework: Vite
- Build command: `npm run build`
- Output directory: `dist`

## MVP limitations

- Heuristic scoring, not a certified judge.
- Works best with full body visible, good light, camera at waist/chest height.
- Back poses cannot truly verify that the user is facing away without a more advanced model; this MVP scores silhouette/limb structure.

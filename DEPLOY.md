# Deploy the web app

This is a static React + Vite app. Camera access works on `localhost` for development, but a public web app must be served over HTTPS.

## Fastest option: Vercel

1. Create a GitHub repository and upload this folder.
2. Go to Vercel and import the repository.
3. Use these settings if Vercel does not auto-detect them:
   - Framework: Vite
   - Build command: `npm run build`
   - Output directory: `dist`
4. Deploy.
5. Open the HTTPS URL on desktop or mobile and allow camera permission.

The included `vercel.json` already sets the build/output and a camera permission header.

## Netlify option

1. Create a GitHub repository and upload this folder.
2. Import the repository into Netlify.
3. Use:
   - Build command: `npm run build`
   - Publish directory: `dist`
4. Deploy.

The included `netlify.toml` sets these automatically.

## Local production test

```bash
npm install
npm run build
npm run start
```

Then open the local preview URL.

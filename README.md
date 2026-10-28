# China Academic World — Railway-ready website

This project packages the website as a small Node.js static server so it can be deployed from GitHub to Railway.

## Files
- `index.html` — the website
- `server.js` — serves the website on Railway's assigned `PORT`
- `package.json` — start command (`npm start`)
- `railway.json` — Railway build and health-check settings
- `.gitignore` — ignores local-only files

## Run locally
Install Node.js 18 or newer, then run:

```bash
npm start
```

Open `http://localhost:3000`.

## Deploy with GitHub + Railway
1. Download and extract this ZIP.
2. Create a new GitHub repository.
3. Upload the **contents** of this folder to the repository root. `index.html`, `package.json`, `server.js`, and `railway.json` should be at the top level, not inside another nested folder.
4. Push/commit the files to GitHub.
5. Sign in to Railway and choose **New Project → Deploy from GitHub Repo**.
6. Connect the repository and start the deployment.
7. When deployment succeeds, open the Railway service's **Settings → Networking** and select **Generate Domain**.
8. Open the generated `https://....up.railway.app` domain.

Railway reads the `npm start` script and uses its assigned `PORT`. No extra environment variables or external packages are required.

## Before publishing
- Check the contact details in the `#contact` section of `index.html`.
- Confirm all university details, rankings, program availability, scholarship information, and deadlines against official sources.
- This is an informational website, not an official university or visa authority website.

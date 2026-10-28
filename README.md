# China Academic World — Updated Railway Deployment Package

This is the updated GitHub + Railway-ready website.

## What's updated
- Removed university-specific "visit official/main site" buttons.
- Added campus photographs for all 10 listed universities.
- Clicking a university photo or **View full details** opens an internal profile panel.
- Each profile includes overview, popular study areas, facilities, typical academic qualifications, admission guidance, document checklist, teaching-language notes, scholarship pathways, and campus/location notes.
- Search, subject/degree filters, and side-by-side comparison remain available.
- The website is responsive for mobile and desktop.

## Files
- `index.html` — website UI and university information
- `server.js` — Node.js static server compatible with Railway's assigned `PORT`
- `package.json` — `npm start` command
- `railway.json` — Railway build and health-check settings
- `.gitignore` — local-only files
- `README.md` — this guide

## Run locally
Install Node.js 18 or newer, open a terminal in this folder, and run:

```bash
npm start
```

Then open `http://localhost:3000`.

## Deploy with GitHub + Railway
1. Download and extract this ZIP.
2. Create a GitHub repository.
3. Upload the **contents** of this folder to the repository root. `index.html`, `server.js`, `package.json`, and `railway.json` should be at the root, not nested inside another folder.
4. Commit/push the files.
5. Sign in to Railway and choose **New Project → Deploy from GitHub Repo**.
6. Connect the repository and deploy.
7. In the Railway service, open **Settings → Networking → Generate Domain**.
8. Open the generated HTTPS domain.

Railway uses the `npm start` command and the assigned `PORT`. No external Node packages are needed.

## Important information
- Campus photographs are loaded from image URLs hosted by universities or image publishers. The visitor needs internet access to see them. If a publisher blocks external image loading, the profile shows a designed fallback instead.
- University program availability, teaching language, admission tests, eligibility, tuition, scholarships and deadlines differ by intake and department. The details are general guidance; verify requirements before applying.
- Rankings shown are overall QS World University Rankings 2027 ranks, not subject-specific ranks. A leading `=` indicates a tied rank.
- Before publishing, verify the business contact details and confirm you have permission to use the China Academic World name and branding.

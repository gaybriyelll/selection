# MIS Operations Portal

A single-page launcher for the MIS systems: Midas (Cleaner and Link), Atmos Website Card, SMS and CIC.

Plain HTML, CSS and JavaScript. No build step and no dependencies.

## Files

- `index.html` is the whole app.
- `vercel.json` sets basic security headers for Vercel.

## Deploy

1. Create a new GitHub repository and upload these files (or run `git init`, `git add .`, `git commit`, `git push`).
2. In Vercel, choose **Add New > Project** and import the repository.
3. Leave the framework preset as **Other**. Leave the build command and output directory empty. Click **Deploy**.

Every push to the main branch redeploys automatically.

## Change the links

The system links are in the `URLS` object near the bottom of `index.html`. Edit the addresses there and push.

## Midas Cleaner

The cleaner is an HTML file you choose from your computer the first time you click **Midas Cleaner**. The portal keeps a copy in that browser's storage (IndexedDB) and opens it in a new tab each time. Nothing is uploaded to the server or to GitHub, so each browser or device needs the file chosen once. Use **Replace file** on the Midas screen to load a newer version.

## Private by default

The Atmos, SMS and CIC addresses are in the page source. If this repository or the Vercel site is public, anyone can see them. Use a private repository and Vercel's deployment protection if the links should not be public.

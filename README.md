# MIS Operations Portal

A single-page launcher for the MIS systems: Midas (Cleaner and Link), Atmos Website Card, SMS and CIC.

Plain HTML, CSS and JavaScript. No build step and no dependencies.

## Files

- `index.html` is the portal.
- `cleaner.html` is the Midas Cleaner (Report Cleaner). It is the original file, unchanged. Do not edit it here unless you mean to replace it.
- `vercel.json` sets basic security headers for Vercel.

## Deploy

1. Create a new GitHub repository and upload these files (or run `git init`, `git add .`, `git commit`, `git push`).
2. In Vercel, choose **Add New > Project** and import the repository.
3. Leave the framework preset as **Other**. Leave the build command and output directory empty. Click **Deploy**.

Every push to the main branch redeploys automatically.

## Change the links

The system links are in the `URLS` object near the bottom of `index.html`. Edit the addresses there and push.

## Midas Cleaner

The **Midas Cleaner** card opens `cleaner.html`, which is deployed with the site. To update the cleaner later, replace `cleaner.html` with the new file (keep the same name) and push. The cleaner loads its Excel libraries from cdnjs, so it needs an internet connection.

## Private by default

The Atmos, SMS and CIC addresses are in the page source. If this repository or the Vercel site is public, anyone can see them. Use a private repository and Vercel's deployment protection if the links should not be public.

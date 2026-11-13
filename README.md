# Getrite Digital — getritedigital.com

Website for Getrite Digital, hosted on Cloudflare Pages.

## Files
- `index.html` — homepage (plans $49.99 / $89.99 / $149.99 per month, ad-spend note, Business Protection Packet download, footer links)
- `privacy.html` — Privacy Policy, live at /privacy
- `copyright.html` — Copyright Form, live at /copyright
- `business-protection-packet.pdf` — Digital Marketing Business Protection Packet (12 forms), live at /business-protection-packet.pdf
- `logo.png` — site logo

Contact: Getritedigital@gmail.com (email only — no phone number on the site)

## How to use this repo
1. Create a new repository on GitHub, e.g. `getrite-digital-site` (do not add a README there, this one already has it).
2. In this folder, run:
   ```
   git remote add origin https://github.com/YOUR-USERNAME/getrite-digital-site.git
   git branch -M main
   git push -u origin main
   ```
   Replace YOUR-USERNAME with your GitHub username.
3. In Cloudflare: Workers & Pages → getritedigital → Settings → Build → Connect to Git, pick this repo, production branch `main`, build output directory `/` (no build step — this is a static site).
4. After that, every time you push a change to `main` on GitHub, Cloudflare will redeploy getritedigital.com automatically. No more manual uploads.

## Making a change
Edit the HTML file, then:
```
git add .
git commit -m "Describe the change"
git push
```

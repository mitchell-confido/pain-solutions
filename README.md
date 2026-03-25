# Dr. Demetrio Aguila - Shingles Pain Surgeon Website

Static website for Dr. Demetrio Aguila's peripheral nerve surgery practice (Total Pain Solutions, Omaha NE).

## Project Structure

```
draguila-site/
  index.html        # Full website (single-page, self-contained)
  netlify.toml      # Netlify deployment config
  .gitignore
  README.md
```

## Preview Locally

Open `index.html` directly in any browser — no server required.

Alternatively, use any static server:

```bash
# Python
python3 -m http.server 8000

# Node (npx, no install)
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to GitHub

```bash
cd draguila-site
git init
git add .
git commit -m "Initial commit: Dr. Aguila website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

## Deploy to Netlify from GitHub

1. Log in to [Netlify](https://app.netlify.com)
2. Click **"Add new site"** > **"Import an existing project"**
3. Connect your GitHub account and select the repository
4. Settings:
   - **Branch to deploy:** `main`
   - **Build command:** *(leave blank)*
   - **Publish directory:** `.`
5. Click **Deploy site**

Netlify will auto-deploy on every push to `main`.

## External Dependencies

The site loads these resources from CDNs (no local copies needed):

- **Google Fonts:** Cormorant Garamond, DM Sans, DM Mono
- **YouTube thumbnails:** 3 video preview images from `img.youtube.com`

All other images are base64-encoded directly in the HTML.

## External Links

The site links to these third-party services:

- Calendly (appointment booking)
- YouTube (patient testimonial videos)
- Facebook (community group)
- Google Maps (office location)
- totalpainsolutions.net (privacy/HIPAA policies)

## Notes

- The HTML file is ~890KB due to base64-embedded images
- No build step is required — this is a purely static site
- All CSS and JS are embedded in the HTML file

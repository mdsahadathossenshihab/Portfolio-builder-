# FolioForge Portfolio Builder — revised frontend MVP

## Included
- Profession-specific themes for Web Developer, Video Editor and Digital Marketer
- Distinct visual palettes, animated hero, hover effects, animated page transitions and scroll reveals
- Profile image, project thumbnail and service image upload from the user's device (max 2 MB each)
- Full-screen Preview button in the top header; preview has clickable Home, About, Work, Services and Contact views and Desktop/Mobile width controls
- Browser-local draft autosave
- Publish modal that checks for `POST /api/portfolios` and clearly reports when the backend is not connected
- GitHub/Vercel-ready static files

## Deploy
Upload `index.html`, `builder.html`, `templates.html`, and `vercel.json` to the root of a GitHub repository. Import the repository in Vercel. Use Framework Preset `Other`, leave Build Command blank, set Output Directory to `.` and deploy.

## Important: automatic publishing needs a backend
This is still a frontend MVP. It does not yet store user accounts or portfolios centrally. Automatic URLs such as `username.yourdomain.com` require a backend API, database, image storage, routing and DNS/domain configuration. The Publish button checks `/api/portfolios`; this project intentionally does not claim a portfolio is live unless that API returns a public URL. Browser image uploads are currently stored as data URLs in localStorage; production should use object storage.

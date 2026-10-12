# FolioForge — Portfolio Builder MVP

A responsive, animated, multi-page static website for Bangladeshi freelancers. Built with plain HTML, CSS and JavaScript so it can be pushed to GitHub and deployed on Vercel without a build step.

## Pages
- `index.html` — landing page and product overview
- `templates.html` — template library
- `builder.html` — portfolio editor with live preview

## Features in this MVP
- Three profession-specific portfolio styles: Web Developer, Video Editor and Digital Marketer
- Live editing of profile, contact information, social links, services and project samples
- Optional profile photo upload (2 MB limit) and project thumbnail URLs
- Desktop/mobile preview toggle
- Local browser draft saving with `localStorage`
- Export a standalone portfolio HTML file
- Responsive layouts, hover transitions, scroll reveal, loading animation and reduced-motion support
- Free subdomain/custom domain fields as draft settings

## Run locally
Open `index.html` in a browser, or use VS Code's Live Server extension.

## Deploy using GitHub + Vercel
1. Create a GitHub repository and upload all files from this folder to its root.
2. In Vercel, choose **Add New → Project** and import the GitHub repository.
3. Set Framework Preset to **Other**. Leave Build Command empty and Output Directory as `.`.
4. Deploy. Future pushes to the connected production branch will trigger deployments.

## Important MVP limitations
This is a front-end prototype. Drafts are saved only in the current browser; there is no account system, shared database, cloud image storage, or multi-user dashboard yet. The domain fields do not automatically provision subdomains, connect DNS or publish a user's portfolio. Exported HTML can be deployed as a static site. A production platform needs authentication, a database/storage layer, per-user public portfolio routes, and server-side/hosting API integration for automated publishing and custom domains.

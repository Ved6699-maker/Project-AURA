# Project AURA ✦

A responsive, installable web-app foundation for a customizable AI companion, designed to expand to Android and Windows.

## Included
- Responsive desktop and mobile interface
- Custom companion name, appearance theme, conversation tone, and browser voice selection
- CSS animated avatar actions: wave, nod, dance, listen
- Browser text-to-speech and speech recognition where supported
- Simple local demo replies
- PWA manifest and service-worker shell caching

## Important limitations
This is an early UI prototype, not yet a full online AI assistant. Without a backend, replies use simple local demo logic. The avatar is a CSS illustration, not a photorealistic or true 3D model. Speech recognition support varies by browser.

## Preview locally
Run a local server in this folder:
    python -m http.server 8080
Then open http://localhost:8080. PWA features require HTTP or HTTPS.

## Publish with GitHub Pages
1. Open Settings → Pages in this repository.
2. Choose Deploy from a branch.
3. Select branch main and folder /(root), then Save.
4. Wait for GitHub Pages to publish the site.

## Online AI next stage
GitHub Pages hosts frontend files only; it cannot run the backend needed to call an online AI API securely. The next stage needs a separate backend with a server-side API key stored in the hosting provider's environment variables. Never commit API keys to this public repository or put them in browser JavaScript.

## Android and Windows
- Android: after the hosted site is stable, package it with a trusted PWA wrapper such as Capacitor.
- Windows: install the PWA from Microsoft Edge or Chrome; a desktop wrapper can be considered later.
- Keep API keys on the backend, not in the public repository.

## Privacy
Do not enter passwords, financial details, or sensitive personal information in this prototype. Preferences are stored in your browser's local storage.

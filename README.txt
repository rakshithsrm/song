NOIR MUSIC — OFFLINE MUSIC PLAYER
=================================

FEATURES
- Add audio files from your computer or phone.
- Tracks are saved in browser IndexedDB and can play without internet.
- Import direct audio file URLs while online (subject to server CORS/download permissions).
- Search, liked songs, playlists, shuffle, repeat, seek and volume controls.
- Installable PWA shell; service worker caches the app interface.

IMPORTANT
This app does not download songs from Spotify, Apple Music, YouTube Music or other
subscription/DRM streaming services. Those services protect their catalogues.
Only import or download audio that you own or are legally allowed to save.
A URL must point directly to an audio file; many websites block browser downloads
with CORS or require authentication.

RUN LOCALLY
1. Extract the ZIP.
2. Open a terminal in the extracted folder.
3. Run a local web server:
   Python:  python -m http.server 8000
4. Open http://localhost:8000 in Chrome or Edge.
   (Do not simply double-click index.html; service workers require localhost/HTTPS.)

INSTALL ON ANDROID
1. Host the folder on an HTTPS static host (or run on localhost for testing).
2. Open the website in Chrome.
3. Open browser menu → Install app / Add to Home screen.
4. Add music while online. Once saved, tracks are available offline in that
   browser profile on that device.

HOSTING
You can deploy the folder as a static site on GitHub Pages, Netlify or Cloudflare Pages.
No backend or account is required. For GitHub Pages, upload the extracted files
to a repository and enable Pages in repository Settings.

DATA NOTES
- Audio files are stored locally in the browser's IndexedDB, not uploaded to a server.
- Clearing browser site data may delete your library. Keep original audio files backed up.
- Browser storage quotas vary by device. Large libraries may use substantial space.
- For best results use Chrome, Edge or Firefox on a current device.

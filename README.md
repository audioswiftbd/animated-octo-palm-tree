# AudioSwift — MP3 Converter Website

A responsive, browser-based audio converter built with HTML, CSS, JavaScript and FFmpeg WebAssembly.

## Features
- Convert audio to MP3, WAV or OGG
- Choose MP3 bitrate (64–320 kbps) to reduce output size
- Optional start/end trim in seconds
- Drag-and-drop file selection
- Client-side processing: selected audio is not uploaded to your own server

## Run locally
Because the app uses JavaScript modules, run it from a local web server rather than opening the HTML file directly.

Python:
    python -m http.server 8000

Then open:
    http://localhost:8000

## Free hosting
You can publish this folder using GitHub Pages or Cloudflare Pages:
1. Create a GitHub repository.
2. Upload `index.html` (and this README if desired).
3. In GitHub, open Settings → Pages.
4. Select Deploy from a branch, choose `main` and `/ (root)`, then Save.

Alternatively, import the folder/repository into Cloudflare Pages and use the static-site defaults.

## Notes
- The FFmpeg engine is downloaded from jsDelivr when the user first converts a file, so an internet connection is required for the engine.
- Conversion happens in the visitor's browser. Large files may be slow or run out of memory on low-powered devices.
- This is a starter static website. It has no server-side upload, user accounts, ads, or analytics.

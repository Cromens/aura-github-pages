# AURA Video Editor — Wix + GitHub Pages

This version keeps FFmpeg entirely same-origin on GitHub Pages. Wix embeds the page in an iframe; FFmpeg's browser Worker, wrapper, core JS and WASM are all served from the same GitHub Pages origin.

Runtime assets:
- @ffmpeg/ffmpeg 0.12.10
- @ffmpeg/core 0.12.10 single-thread

The GitHub Actions workflow installs the packages and copies only the required runtime files into `dist/vendor/` before deploying the static site.

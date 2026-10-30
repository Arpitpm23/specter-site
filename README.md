# Specter

Static homepage for [tryspecter.tech](https://tryspecter.tech/).

GitHub Pages publishes the repository root from `main`. Keep `CNAME` and
`.nojekyll` in the root. No package installation or build step is required.

## Local preview

```sh
python3 -m http.server 8769 --bind 127.0.0.1
```

## Temporary visual assets

The background video and poster are Prime Intellect reference assets retained
at the founder's request. They are not original Specter artwork. This repository
does not grant a license to those third-party assets.

Sources:

- https://www.primeintellect.ai/backgrounds/pi-glass-loop-prod.webm
- https://www.primeintellect.ai/backgrounds/pi-glass-loop-prod.mp4
- https://www.primeintellect.ai/backgrounds/pi-glass-loop-poster.webp

Local copies in `assets/` let the homepage serve its media without hotlinking.
The still poster is also used when the viewer requests reduced motion.

`glass-island-loop-fast.mp4` is a 720p H.264 derivative of the source MP4,
encoded without audio and with the MP4 index at the start for progressive playback.
It retains the moving section from 4.5 to 13.5 seconds, trimming the long still holds.
The scene image stays visible independently until the video has a decoded frame.

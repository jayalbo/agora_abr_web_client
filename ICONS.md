# App Icon Guide

Default icon file used by the web app:

- `assets/icons/app-icon.svg`

If you want to replace the icon with PNG files, put them here:

- `assets/icons/favicon-32.png` (32x32)
- `assets/icons/favicon-192.png` (192x192)
- `assets/icons/favicon-512.png` (512x512)

PNG requirements:

- Use exact square sizes listed above.
- Use transparent background if desired.
- Use `sRGB` color profile.
- Keep each file under 500 KB.

How to switch from SVG to PNG:

1. Open `index.html`.
2. Keep or remove the SVG line:
   - `<link rel="icon" type="image/svg+xml" href="./assets/icons/app-icon.svg" />`
3. Add PNG icon lines in `<head>`:

```html
<link rel="icon" type="image/png" sizes="32x32" href="./assets/icons/favicon-32.png" />
<link rel="icon" type="image/png" sizes="192x192" href="./assets/icons/favicon-192.png" />
```

Optional for PWA/home-screen support:

- also include `favicon-512.png` in a web manifest.

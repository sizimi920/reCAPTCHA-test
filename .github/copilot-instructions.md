# reCAPTCHA Demo Project - AI Coding Guidelines

## Project Overview

This is a simple Japanese-language reCAPTCHA demo application - a single-page web app that validates users as human using Google's reCAPTCHA v2 service.

## Architecture & Structure

- **Pure frontend**: No build tools, frameworks, or backend dependencies
- **Static files**: `index.html`, `script.js`, `style.css` - deploy directly to any web server
- **External dependency**: Google reCAPTCHA API loaded via CDN (`https://www.google.com/recaptcha/api.js`)

## Key Components

### HTML (`index.html`)

- **Language**: Japanese (`lang="ja"`) - all user-facing text is in Japanese
- **reCAPTCHA integration**: Uses `data-sitekey` and `data-callback` attributes on `.g-recaptcha` element
- **Site key**: `6Lc6CLMrAAAAADz0W43HhfzahZV14C3ErwQh2FC-` (hardcoded for demo)

### JavaScript (`script.js`)

- **Callback pattern**: `onHumanVerified()` function is called by reCAPTCHA API on successful verification
- **DOM manipulation**: Shows success message by toggling `display` style property
- **No error handling**: Intentionally minimal for demo purposes

### CSS (`style.css`)

- **Design system**: Uses Poppins font, gradient background (`#74ABE2` to `#5563DE`), centered card layout
- **Animation**: CSS `fadeIn` keyframes for card entrance effect
- **Hidden state**: Success message (`.greeting`) starts with `display: none`

## Development Patterns

- **No JavaScript modules**: All code is in global scope for simplicity
- **No CSS preprocessors**: Plain CSS with modern features (flexbox, gradients, animations)
- **Minimal JavaScript**: Single callback function, direct DOM access with `getElementById`

## Testing & Deployment

- **Local testing**: Open `index.html` directly in browser (file:// protocol works)
- **Production**: Serve from any static web server (GitHub Pages, Netlify, etc.)
- **reCAPTCHA testing**: Works on localhost and file:// - no HTTPS required for development

## When Making Changes

- Keep Japanese language consistency in user-facing text
- Maintain minimal dependency approach - avoid adding build tools
- reCAPTCHA site key is demo-only - replace for production use
- CSS animations should maintain the smooth, professional feel

## File Dependencies

- `index.html` → `style.css`, `script.js`, Google reCAPTCHA API
- `script.js` → Called by reCAPTCHA API, manipulates DOM elements defined in HTML
- `style.css` → Standalone, no external dependencies beyond Google Fonts

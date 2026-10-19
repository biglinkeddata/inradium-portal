# Inradium portal

Company website for Inradium Limited. A single static page with no build step.

## Structure

- `index.html` - the whole site: markup, CSS and JS inline
- `assets/` - logos, hero video and stills, character illustrations
- `netlify.toml` - publish directory and cache/security headers

## Hero background

The hero picks its background by screen shape:

- landscape screens: `assets/hero-landscape.mp4`
- near-square (tablet): `assets/hero-tablet.webp`
- portrait phones: `assets/hero-portrait.mp4` with `assets/hero-portrait.webp` as the poster

## Deploy

Netlify, publishing the repo root. Connect the repo in Netlify and every push to `main` deploys.

Manual deploy: `npx netlify-cli deploy --prod --dir=.`

## Still to wire up

The contact and subscribe forms only show a client-side confirmation. Add `data-netlify="true"` to both `<form>` elements to use Netlify Forms, or point them at a backend.

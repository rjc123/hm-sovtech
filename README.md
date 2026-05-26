# Sovereign Tech Stack — website

The website for the Sovereign Tech Stack venture — a certification platform assembling a complete UK-owned technology stack for British SMEs.

**Live:** https://sovtech.theprivatealpha.com

## What this venture is

British businesses run almost entirely on American infrastructure — from DNS and hosting through email, documents, CRM, payments, and AI. Sovereign Tech Stack is a certification body and curated marketplace assembling a complete UK-owned alternative. Not advocacy, not policy, not a directory — a purchasable answer to *what should we use instead?*

The site is currently a pre-launch preview, gated behind an access code while the thesis is finalised and the strategic partner conversation opens. Request access via [robin@robincarswell.com](mailto:robin@robincarswell.com?subject=Sovereign%20Tech%20Stack%20—%20preview%20access&body=Please%20send%20the%20preview%20access%20code%20for%20sovtech.theprivatealpha.com.%0A%0AName%3A%0AAffiliation%3A%0AContext%3A%0A).

## This repository

Static site built with [Hugo](https://gohugo.io) extended and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

```
content/        page content (Markdown + front matter)
layouts/        Hugo template overrides
assets/css/     brand stylesheet
static/         static assets, including CNAME for custom domain
themes/         git submodules: PaperMod, sam
config.toml     site configuration
```

## Local development

Requires Hugo extended 0.161.0 or later.

```sh
git clone https://github.com/rjc123/hm-sovtech.git
cd hm-sovtech
git submodule update --init --recursive
hugo server
```

Visit http://localhost:1313 — you will see the access-code prompt before the site renders.

## Deployment

Pushes to `main` deploy automatically via [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml). The workflow installs Hugo, builds the site, and publishes to GitHub Pages with the custom domain from `static/CNAME`.

## Licence

All content is © Sovereign Tech Stack. Code in this repository is unlicensed pending a decision on the venture structure.

# Estimara Media

Public image host for Estimara marketing carousels.

This repository exists for one reason: the Instagram and Facebook Content Publishing APIs **fetch images from a public URL** — they do not accept uploaded image bytes. The Jarvis repo that generates these carousels is private, so its raw URLs can't be fetched by Meta. This repo is the public mirror that solves that.

## What's in here

Only **rendered carousel output** — JPGs produced by `scripts/carousel_pipeline.py` in the Jarvis repo:

```
carousels/<carousel-id>/instagram/slide-N.jpg    1080x1350
carousels/<carousel-id>/tiktok/slide-N.jpg       1080x1920
```

## What is deliberately NOT in here

No source, no business data, no revenue or ad figures, no credentials, no `carousel.json` manifests. Nothing but finished marketing images that are intended to be published publicly anyway.

## How it's updated

Automatically, by `scripts/sync_media.py` in the private Jarvis repo. Don't hand-edit — changes will be overwritten on the next sync.

Served via GitHub Pages at https://midwestcapitalsolutions.github.io/estimara-media/

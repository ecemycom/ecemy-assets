# Ecemy Assets

Assets submodule for [ecemy-engine](https://github.com/ecemycom/ecemy-engine).

This repository contains only the **assets** (images, screenshots, diagrams)
extracted from vendor snapshot folders. The directory structure mirrors the
main repo exactly — only the `assets/` directories are synced.

## How it works

1. Place images into `content/{category}/{slug}/{date}/assets/` in the main repo.
2. Run `./scripts/sync-assets.sh` from the main repo to rsync assets here.
3. Run `./scripts/push-assets.sh` to commit and push this submodule to GitHub.

## URLs on CDN

Assets are served via jsDelivr at:

```
https://cdn.jsdelivr.net/gh/ecemycom/ecemy-assets/content/{category}/{slug}/{date}/assets/{filename}
```

## Ownership

| Repo         | Owner    | Purpose                                   |
| ------------ | -------- | ----------------------------------------- |
| ecemy-engine | ecemycom | Main pipeline, metadata, and source files |
| ecemy-assets | ecemycom | CDN-hosted asset files only               |

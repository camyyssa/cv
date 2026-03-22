# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal CV/resume site for Camelia Smeria, hosted at https://camyyssa.github.io/cv/. CV content is defined in `index.yml` and rendered to `index.html` using the `turtle-cv` tool.

## Build

```
pnpm install      # install dependencies
pnpm build        # builds index.html from index.yml (runs turtle-cv with --watch)
```

## How It Works

- `index.yml` — CV data (profile, work history, education, languages, social links)
- `index.html` — generated output (committed to repo for GitHub Pages deployment)
- `turtle-cv` — external dependency that converts the YAML into a styled HTML page

To update the CV, edit `index.yml` and run `pnpm build` to regenerate `index.html`. Both files must be committed and pushed to master for deployment.

## Deployment

Push to `master` triggers GitHub Pages deployment automatically.

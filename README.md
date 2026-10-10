# FetchGUI

A browser-based visual editor for creating and exporting Fastfetch configurations.

## Current features

- Live terminal preview
- Toggle modules and rearrange the order
- Choose a built-in logo source, key color, separator, and key width
- buit-in presets templates: Balanced, Minimal, and Classic
- Generate Fastfetch JSONC. copy it or download `config.jsonc`

> The terminal preview uses sample values. It does not inspect the computer running the browser. The generated configuration should be tested with your installed Fastfetch version before replacing an existing config.

## Requirements

- Node.js 20 or later
- npm

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Vite, usually `http://localhost:5173`.


## Test the generated config

Download `config.jsonc` from the app and test it without replacing your current configuration:

```bash
fastfetch --config ./config.jsonc
```

If it behaves as expected, back up your existing config and then copy it into `~/.config/fastfetch/config.jsonc`.

## Upcoming Goals

- Import an existing `config.jsonc`  into the editor
- Per-module options and custom labels / format strings
- User-defined ASCII art and local image logos
- More color schemes and per-module color pickers
- Validation against Fastfetch's JSON schema
- Shareable config links

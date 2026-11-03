# Gruvbox

Modernized Gruvbox themes with 3 contrast variations (hard, medium, soft) across both Dark and Light modes on Herdr's default layout, paired with pure monochrome icons for AI models and developer tools.

![Gruvbox](preview.png)

## What you see

- **Dark Mode (`gruvbox`, `gruvbox-medium`, `gruvbox-soft`):**
  - **Buffers & Cards:** Signature dark buffer backgrounds (`#1d2021` hard, `#282828` medium, `#32302f` soft) with 1px `#3c3836` borders and bright `#fe8019` focus outlines.
  - **Sidebars & Chrome:** Darkened backdrops (`#161819` hard, `#212324` medium, `#282828` soft) for visual hierarchy and depth.
  - **Text & Syntax:** Crisp `#ebdbb2` foreground, `#a89984` muted, and `#7c6f64` dim text.
  - **Agent Statuses:** Yellow (`#fabd2f`) working, red (`#fb4934`) blocked, aqua (`#8ec07c`) done, gray (`#928374`) idle.
- **Light Mode (`gruvbox-light`, `gruvbox-light-medium`, `gruvbox-light-soft`):**
  - **Buffers & Cards:** Warm light buffer backgrounds (`#f9f5d7` hard, `#fbf1c7` medium, `#f2e5bc` soft) with 1px `#d5c4a1` borders and rust `#af3a03` focus outlines.
  - **Sidebars & Chrome:** Warm chrome backdrops (`#ebdbb2` hard, `#f2e5bc` medium, `#ebdbb2` soft).
  - **Text & Syntax:** Dark `#3c3836` foreground, `#7c6f64` muted, and `#928374` dim text.
  - **Agent Statuses:** Warm yellow (`#b57614`) working, red (`#9d0006`) blocked, blue (`#076678`) done, gray (`#928374`) idle.
- **Monochrome Icons:**
  - AI model icons (Claude, Gemini, Antigravity, Codex, Amp, Crush, Kimi, Kiro, Pig) render as pure monochrome glyphs tinted to the active theme's foreground/muted text colors, blending cohesively with Neovim, Vim, Git, and Shell without distracting brand colors or color schemes.

## How it behaves

- Pure theme support: relies entirely on Herdr's native semantic tokens (`canvas`, `background`, `surface`, `chrome`, `border`, `accent`, etc.) on the default layout (`main`).
- Switch cleanly between any of the 6 variants at any time without layout modifications or overrides.
- Optional monochrome icons via `programs.json` and `icons-mono/`.

## Built from

- **Themes (`themes/`):**
  - `themes/gruvbox.json`: Hard contrast dark Gruvbox palette (default).
  - `themes/gruvbox-medium.json`: Medium contrast dark Gruvbox palette.
  - `themes/gruvbox-soft.json`: Soft contrast dark Gruvbox palette.
  - `themes/gruvbox-light.json`: Hard contrast light Gruvbox palette (default light).
  - `themes/gruvbox-light-medium.json`: Medium contrast light Gruvbox palette.
  - `themes/gruvbox-light-soft.json`: Soft contrast light Gruvbox palette.
- **Monochrome Icons:**
  - `icons-mono/`: Clean single-path monochrome vector glyphs for AI models.
  - `programs.json`: Overrides AI model programs with `tint: true`.

## Done when

1. Theme files exist in `themes/` and install cleanly to `~/.config/herdr-app/themes/`.
2. All 6 variants apply cleanly with 0 errors on the default layout:
   - `herdr-app do app.theme --name gruvbox`
   - `herdr-app do app.theme --name gruvbox-medium`
   - `herdr-app do app.theme --name gruvbox-soft`
   - `herdr-app do app.theme --name gruvbox-light`
   - `herdr-app do app.theme --name gruvbox-light-medium`
   - `herdr-app do app.theme --name gruvbox-light-soft`
3. Copying `icons-mono/` and `programs.json` into `~/.config/herdr-app/` renders all AI models with theme-tinted monochrome icons.
4. No custom layout files or overrides are needed.

# Phosphor Green for Orca

A dark Orca theme inspired by 1980s green-phosphor terminals. Near-black surfaces, green text, and a bright cursor carry through the app, editor, and terminal. Syntax highlighting and ANSI colors use different greens and levels of brightness.

## Install locally

The app and terminal palettes require Orca 1.4.246 or later. The optional scanline texture uses Orca's theme background support, validated on 1.4.277.

1. Open **Settings → Plugins**, turn on plugins, then choose **Development folders…** and add this repository's root folder.
2. In **Settings → Appearance**, set the theme mode to **Dark** and choose **Phosphor Green** for **Dark theme**.
3. In **Settings → Terminal**, choose **Phosphor Green** for **Dark Theme**.

You can also load the folder from a terminal opened here with `orca plugin dev load .`.

For scanlines, set the terminal's **Background Opacity** to about **70%** in Terminal settings. Orca shows the texture behind translucent terminals and agent chats. You can also select a **Block** cursor and a monospace font such as **Consolas**. Phosphor bloom and screen curvature require renderer support.

## Plugin files

| File | Purpose |
| --- | --- |
| [`orca-plugin.json`](orca-plugin.json) | Data-only manifest registering both themes |
| [`themes/phosphor-green.json`](themes/phosphor-green.json) | Dark app colors and TextMate syntax styles |
| [`terminal/phosphor-green.json`](terminal/phosphor-green.json) | Terminal colors, including the full ANSI palette |
| [`images/scanlines.png`](images/scanlines.png) | Tileable scanline background |

Run `orca plugin validate .` from this folder to check the manifest and both contributions.

The layout follows the official plugin example. Orca documents the theme fields and where the background appears. [Orca OLED plugin](https://github.com/stablyai/orca-plugins/tree/3ad7e2c36acf9fabb4148b99359dca95d345ba4c/plugins/oled-theme) · [Orca theme reference](https://github.com/stablyai/orca/blob/main/docs/reference/plugin-themes.md)

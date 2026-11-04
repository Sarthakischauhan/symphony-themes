# Symphony Themes

Native, data-only color themes for the [Symphony coding agent](https://github.com/Sarthakischauhan/symphony). This plugin contains no skills, tools, or executable addon code.

## Themes

- **One Dark** — a dark palette based on Atom's One Dark colors.
- **Symphony Dusk** — an original purple-tinted dark palette.
- **Symphony Daylight** — an original light palette.

## Install

Theme plugins require the Symphony `feat/plugin-themes` branch until that feature is released. From that checkout:

```sh
uv run symphony plugins add Sarthakischauhan/symphony-themes
uv run symphony themes list
uv run symphony
```

Inside Symphony, use `/theme` to preview and select a theme, or use `/theme symphony-themes:One Dark` directly. Changes take effect in new sessions after installation. To update or remove the plugin:

```sh
uv run symphony plugins update symphony-themes
uv run symphony plugins remove symphony-themes
```

An existing `$SYMPHONY_HOME/theme.toml` (or `~/.symphony/theme.toml`) overrides the selected plugin theme and is never overwritten.

## Contribute a theme

Add a uniquely named TOML file under `themes/`, with `name`, `base` (`dark` or `light`), and a `[colors]` table. Existing files show all supported tokens. Specify every token for predictable colors; missing tokens fall back to the selected base palette. Only theme data is read; CSS and executable code are not loaded from theme files.

Some Symphony widgets still use fixed colors, and transcript text already rendered before switching themes may keep its old colors. Contributions must be your own or include clear licensing and attribution.

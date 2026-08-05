# Tabby Quick Cmd Buttons

A Tabby terminal plugin that displays your **Quick Commands** as a compact, draggable button panel.

This fork modernizes the original plugin UI so it follows Tabby's active theme instead of using fixed colors and an unrelated component theme.

## Features

- Quick Command groups shown as tabs
- Command buttons that follow Tabby's current theme
- Active tab can be clicked again to collapse its command list
- Compact minimize / restore behavior
- Add, edit and delete Quick Commands from the panel
- **Edit first** mode to insert a command without immediately pressing Enter
- Draggable and resizable panel
- Light/dark/custom Tabby theme support

## Requirement

Install **tabby-quick-cmds** first and create Quick Commands there. This plugin uses the commands stored in Tabby's `qc.cmds` configuration.

## Development install

For local testing, clone this repository directly into Tabby's plugin modules directory and build it.

Windows example:

```bat
cd %APPDATA%\tabby\plugins\node_modules
git clone -b theme-modernization https://github.com/danhk0612/tabby-quick-cmds-buttons.git
cd tabby-quick-cmds-buttons
npm install
npm run build
```

Restart Tabby after building.

To update an existing development install:

```bat
git pull
npm install
npm run build
```

## Build

```bash
npm ci
npm run build
```

Compiled files are written to `dist/`.

## Publishing

Publishing is handled by GitHub Actions when a release tag is pushed. The repository must have an `NPM_TOKEN` secret with permission to publish the configured npm package.

## Upstream

This repository is a fork of Richard's original project:

- https://github.com/weijia/tabby-quick-cmds-buttons/

The original plugin was based on Eugene Pankov's `tabby-clippy` work.

## License

MIT. The original copyright and license notice are retained in [LICENSE](./LICENSE).

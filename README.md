# Tabby Quick Cmd Buttons Modern

A modernized Tabby terminal plugin that displays your **Quick Commands** as a compact, draggable button panel.

This fork updates the original plugin UI so it follows Tabby's active theme instead of using fixed colors and an unrelated component theme.

## Features

- Quick Command groups shown as tabs
- Command buttons that follow Tabby's current theme
- Active tab can be clicked again to collapse its command list
- Compact minimize / restore behavior
- Add, edit and delete Quick Commands from the panel
- **Edit first** mode to insert a command without immediately pressing Enter
- Draggable and resizable panel
- Light, dark and custom Tabby theme support

## Requirement

Install **tabby-quick-cmds** first and create Quick Commands there. This plugin uses the commands stored in Tabby's `qc.cmds` configuration.

## Installation

After the npm package is published, install **tabby-quick-cmds-buttons-modern** from Tabby's plugin manager.

For development or local testing, clone this repository directly into Tabby's plugin modules directory and build it.

Windows example:

```bat
cd %APPDATA%\tabby\plugins\node_modules
git clone -b theme-modernization https://github.com/danhk0612/tabby-quick-cmds-buttons-modern.git
cd tabby-quick-cmds-buttons-modern
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

Releases are published to npm from GitHub Actions when a `v*` tag is pushed.

The repository must have an `NPM_TOKEN` Actions secret with permission to publish `tabby-quick-cmds-buttons-modern`.

Release example:

```bash
git tag v1.3.0
git push origin v1.3.0
```

## Upstream

This repository is a fork of Richard's original project:

- https://github.com/weijia/tabby-quick-cmds-buttons/

The original plugin was based on Eugene Pankov's `tabby-clippy` work.

## License

MIT. The original copyright and license notice are retained in [LICENSE](./LICENSE).

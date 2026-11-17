# Stark Theme

A warm, paper-like theme with purple accents. Available in light, dark, and burgundy variants.

## Multi-Editor Support

Stark Theme is designed to provide a consistent experience across multiple code editors. Currently supported:

- **Zed** - Native extension support
- **VS Code** - Full marketplace integration
- **Sublime Text 4** - by leoric

The project is structured to make adding new editor support straightforward. Each editor has its own directory under `editors/` with theme files in the appropriate format.

## Variants

### Stark Light

A warm, cream-toned light theme

![Stark Light](assets/light.png)

### Stark Dark

A cozy dark theme with warm undertones

![Stark Dark](assets/dark.png)

### Stark Burgundy

A deep plum/burgundy theme (`#6B2D5B`) with warm cream/gold foreground and accents (`#E8D5B7`)

## Installation

### Zed

#### From Zed Extensions

1. Open Zed
2. Go to Extensions (cmd+shift+x)
3. Search for "Stark"
4. Click Install

#### Manual Installation

1. Copy the `editors/zed` directory contents to your Zed extensions folder
2. Restart Zed and select the theme from settings

### VS Code

#### From VS Code Marketplace

1. Open VS Code
2. Go to Extensions (cmd+shift+x)
3. Search for "Stark Theme"
4. Click Install

#### Manual Installation

1. Copy the `editors/vscode` directory to `~/.vscode/extensions/stark-theme`
2. Restart VS Code and select the theme from Color Theme settings

#### Building VSIX Package

1. Navigate to the VS Code theme directory:
   ```bash
   cd editors/vscode
   ```
2. Package the extension:
   ```bash
   npx vsce package
   ```
3. Install the generated `.vsix` file in VS Code via Extensions > Install from VSIX

## Install

1. Open `Preferences → Browse Packages…`
2. Copy this folder in, keeping the name `Stark Theme`.
3. Open `Preferences → Theme…` → pick a Stark theme.
4. Open `Preferences → Color Scheme…` → pick the matching Stark scheme.


## Project Structure

```
stark-theme/
├── assets/              # Theme preview images
│   ├── light.png
│   └── dark.png
├── editors/
│   ├── zed/             # Zed editor theme
│   │   ├── extension.toml
│   │   └── themes/
│   │       └── stark.json
│   ├── vscode/          # VS Code theme
│   │   ├── package.json
│   │   └── themes/
│   │       ├── stark-light.json
│   │       └── stark-dark.json
│   └── sublime/          # Sublime Text 4 theme
├── LICENSE
└── README.md
```

## Adding Support for New Editors

To add support for a new editor:

1. Create a new directory under `editors/` with the editor name
2. Add the theme files in the format required by that editor
3. Update this README with installation instructions

## License

MIT

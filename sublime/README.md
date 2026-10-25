# Stark Theme for Sublime Text 4

A Sublime Text 4 port of [Stark Theme](https://github.com/minhtrungcc/stark-theme), a warm, paper-like theme with purple accents. Includes UI themes and syntax color schemes for Light, Dark, and Burgundy variants.

This is an independent community port, not an official release by the original author.

## Included

- `Stark Light.sublime-theme` + `Stark Light.sublime-color-scheme`
- `Stark Dark.sublime-theme` + `Stark Dark.sublime-color-scheme`
- `Stark Burgundy.sublime-theme` + `Stark Burgundy.sublime-color-scheme`

The `.sublime-theme` files style Sublime Text's UI. The `.sublime-color-scheme` files style text and syntax highlighting. Set both to get the complete look.

## Install

1. In Sublime Text, choose **Preferences → Browse Packages…**
2. Create a folder named `Stark Theme`.
3. Copy the contents of this package into that folder, preserving the `themes` and `color-schemes` directories.
4. Open **Preferences → Select Theme…** and choose a Stark variant.
5. Open **Preferences → Select Color Scheme…** and choose the matching Stark variant.

Alternatively, open **Preferences → Settings** and set both settings explicitly. Example for Dark:

```json
{
    "theme": "Stark Dark.sublime-theme",
    "color_scheme": "Packages/Stark Theme/color-schemes/Stark Dark.sublime-color-scheme"
}
```

For Light or Burgundy, replace both filenames with the matching variant.

## Notes

- This is a hand-authored ST4 port. Sublime Text's UI theme API differs from VS Code's workbench theme API, so some editor-specific UI details cannot map one-to-one.
- The color schemes use Sublime Text's native `.sublime-color-scheme` format and common TextMate scopes.
- The Burgundy variant uses a deep plum background with warm cream/gold foreground and purple accents.
- If a UI element does not pick up a custom color, Sublime Text may be using a built-in control that does not expose that color in the theme API.

## Credits and license

Based on the palette and design of **Stark Theme** by minhtrungcc:
https://github.com/minhtrungcc/stark-theme

The upstream project declares the MIT License. See `LICENSE` for the license text and attribution.

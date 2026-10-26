# Stark Theme for Sublime Text 4

A warm, paper-like theme with purple accents, ported from
[minhtrungcc/stark-theme](https://github.com/minhtrungcc/stark-theme).
Variants: **Stark Light**, **Stark Dark**, **Stark Burgundy**.

## Structure

| File | Purpose |
| --- | --- |
| `Stark.hidden-theme` | All UI rules. `extends` `Adaptive.sublime-theme`. Colours are `var(...)` only. |
| `Stark Light/Dark/Burgundy.sublime-theme` | Extend `Stark.hidden-theme` and only redefine the colour variables. |
| `Stark Light/Dark/Burgundy.sublime-color-scheme` | Syntax colour schemes. |
| `Widget - Stark ….sublime-settings` | Make find/input widgets use the matching colour scheme. |

To tweak a colour, edit the variable in the variant's `.sublime-theme`
(e.g. `tabActiveBorder`, `sidebarBackground`); the rules never need to change.

## Install

1. `Preferences → Browse Packages…`
2. Copy this folder in, keeping the name `Stark Theme`.
3. `Preferences → Theme…` → pick a Stark theme.
4. `Preferences → Color Scheme…` → pick the matching Stark scheme.

## Credits

Colours: minhtrungcc/stark-theme (MIT). Rule layout informed by
mauroreisvieira/github-sublime-theme (MIT).

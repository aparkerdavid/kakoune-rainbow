# Kakoune rainbow

Personal fork of JJK96's [kakoune-rainbow](https://github.com/JJK96/kakoune-rainbow), which gains a substantial speed boost at the cost of a more involved and slightly sketchy hook setup.

Highlights pairs of parentheses in the same color, recursive pairs are highlighted in a different color.

# Install

Add this plugin to your `autoload` folder.

Or use [plug](https://github.com/andreyorst/plug.kak)
```
plug 'aparkerdavid/kakoune-rainbow'
```

# Usage

execute `:rainbow` to highlight the current buffer once.

execute `:rainbow-enable` to highlight the current buffer continuously (note that this may be a bit laggy).

execute `:rainbow-disable` to remove the highlighter

# Configuration

The `rainbow_highlight_background` option sets whether the background of the part between braces should be highlighted.

# Customization

You can override the `rainbow_faces` option to set your own faces.

Example:
```
set-option global rainbow_faces "rgb:ff0000" "rgb:00ff00" "rgb:0000ff"
```

You can also override the `rainbow_opening` option to set the opening parentheses regex.
Example:
```
set-option global rainbow_opening "[\[{(<]"
```

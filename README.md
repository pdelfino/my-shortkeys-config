# my-shortkeys-config

![Young Hare](https://upload.wikimedia.org/wikipedia/commons/thumb/4/44/Albrecht_D%C3%BCrer_-_Hare%2C_1502_-_Google_Art_Project.jpg/960px-Albrecht_D%C3%BCrer_-_Hare%2C_1502_-_Google_Art_Project.jpg)

*"Young Hare" (1502) by Albrecht Durer -- [Wikipedia](https://en.wikipedia.org/wiki/Young_Hare)*

**Emacs-flavored keyboard shortcuts for Brave and Chrome.**

Configuration for the [Shortkeys](https://www.shortkeys.app/) browser extension, adding Emacs-style keybindings that complement the system-wide remappings provided by [Karabiner Elements](https://github.com/pdelfino/karabiner-config). Karabiner handles most of the heavy lifting (`C-n`, `C-p`, `C-f`, `C-b`, etc.), so this config covers the browser-specific actions that Karabiner cannot reach.

## Shortcuts

| Shortcut | Emacs Notation | Action |
|---|---|---|
| `Alt+Shift+.` | `M->` | Scroll to bottom of page |
| `Alt+Shift+,` | `M-<` | Scroll to top of page |
| `Ctrl+G` | `C-g` | Google search selected text |
| `Ctrl+Shift+U` | `C-S-u` | Copy current URL to clipboard |

## How It Works

Shortkeys is a browser extension that lets you define custom keyboard shortcuts for browser actions. The JSON configuration below can be imported directly into the extension's settings.

```json
[
  {
    "action": "bottom",
    "key": "alt+shift+.",
    "label": "M->"
  },
  {
    "key": "alt+shift+,",
    "label": "M-<",
    "action": "top"
  },
  {
    "key": "ctrl+g",
    "label": "C-g",
    "action": "searchgoogle"
  },
  {
    "action": "copyurl",
    "key": "ctrl+shift+u",
    "label": "C-shift-u"
  }
]
```

## Installation

1. Install the [Shortkeys extension](https://www.shortkeys.app/) in Brave or Chrome
2. Open the extension settings
3. Import the JSON config above (or copy it into the custom shortcuts editor)

## Why So Few Shortcuts?

Most Emacs navigation keybindings (`C-n`, `C-p`, `C-f`, `C-b`, `C-a`, `C-e`, `C-v`, `M-v`, etc.) are handled at the OS level by [karabiner-config](https://github.com/pdelfino/karabiner-config), so they work everywhere -- including inside the browser. Shortkeys only needs to cover actions that are browser-specific and cannot be intercepted by Karabiner.

## Related

- [karabiner-config](https://github.com/pdelfino/karabiner-config) -- System-wide Emacs keybindings via Karabiner Elements
- [homerow-config](https://github.com/pdelfino/homerow-config) -- Click things without a mouse
- [emacs-config](https://github.com/pdelfino/emacs-config) -- The Emacs setup at the center of this workflow

## License

MIT

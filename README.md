# My shortkeys config

My configuration for the extension caleed shortkeys config available
for Chrome and Brave (I use Brave).

While using macOS, I am using Brave - since Nyxt Browser does not have
official support. Fortunately, Brave has access to all extensions
available for Google Chrome.

One of them is called Shortkeys config. I try having an Emacs UX in
Brave, so this is my config:

Some of my tweaks become unnecessary after I started using
karabiner-elements. For instance, no need to set `C-n` to scroll-up.
[See my config
here](https://github.com/pdelfino/my-karabiner-elements-config).

Also, I am understanding better [Brave
shortcuts](https://support.brave.com/hc/en-us/articles/360032272171-What-keyboard-shortcuts-can-I-use-in-Brave-).
Some are fine to keep, there is no need to change. For instance,
`Command+Shift+ ] or [` to switch between tabs in a hierarchical
manner.


```json
[
  {
    "action": "bottom",
    "key": "alt+shift+.",
    "label": "M->",
    "sites": "",
    "sitesArray": [
      ""
    ]
  },
  {
    "key": "alt+shift+,",
    "label": "M-<",
    "action": "top",
    "sites": "",
    "sitesArray": [
      ""
    ]
  },
  {
    "key": "ctrl+g",
    "label": "C-g",
    "action": "searchgoogle",
    "sites": "",
    "sitesArray": [
      ""
    ]
  },
  {
    "action": "copyurl",
    "key": "ctrl+shift+u",
    "label": "C-shift-u",
    "sites": "",
    "sitesArray": [
      ""
    ]
  }
]
```


# nbpreview.yazi

View your Jupyter notebooks beautifully in the preview in Yazi.

## Requirements

- [Yazi](https://github.com/sxyazi/yazi) version >=0.2.5
- [nbpreview]

## Previews

TODO

## Installation

```bash
## For linux and MacOS
git clone https://github.com/AnirudhG07/nbpreview.yazi.git ~/.config/yazi/plugins/nbpreview.yazi

## For Windows
git clone https://github.com/AnirudhG07/nbpreview.yazi.git %AppData%\yazi\config\plugins\nbpreview.yazi
```

## Usage

After installing the plugin, add this to your `yazi.toml` file inside the plugin's section previously present.

```toml
[plugin]
prepend_previewers = [
  { name = "*.ipynb", run = "nbpreview" },
]
```

## Configurations

You can configure your preview by editing the `init.lua` file present in the plugin directory.

You can see the configurations provided using `nbpreview --help`.

By default we have give you some of the flags which you can change according to your needs in the `init.lua` file.
Please donot change the below options(unless you know what you are doing) -

- `--nerd-font` - Yazi uses nerd-font.
- \*`--decorated` - This enables the decorations you see in the preview.
- `--no-paging` - To avoid errors.

The `OPTIONAL CHANGES` flags are by default(recommended) given. You can add more or change as you wish.

## CUSTOMIZATION

You can Color customize your previews from the Color schemes and themes provided by `nbpreview`. These are -

```bash
# COLOR SCHEMES
--color-system, --cs [standard|256|truecolor|windows|none|auto]
                The type of color system to use.  [env var: NBPREVIEW_COLOR_SYSTEM]

# THEMES
  -t, --theme [abap|algol|algol_nu|arduino|autumn|bw|borland|coffee|colorful|default|dracula|emacs|friendly_grayscale|friendly|fruity|github-dark|gruvbox-dark|gruvbox-light|igor|inkpot|lightbulb|lilypond|lovelace|manni|material|monokai|murphy|native|nord-darker|nord|one-dark|paraiso-dark|paraiso-light|pastie|perldoc|rainbow_dash|rrt|sas|solarized-dark|solarized-light|staroffice|stata-dark|stata-light|tango|trac|vim|vs|xcode|zenburn|light|dark|ansi_light|ansi_dark]
```

You can change the default give color scheme and theme to any you like.

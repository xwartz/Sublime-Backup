
## My Sublime Text 3 Settings Backup

This repository contains my Sublime Text settings.

### Usage

1. `cd ~/Library/Application\ Support/`

2. `git clone git@github.com:xwartz/Sublime-Backup.git`

3. `mv Sublime-Backup/ Sublime\ Text\ 3/`

### More about Sublime Text Syncing
https://packagecontrol.io/docs/syncing

### Settings
```json
{
	"always_show_minimap_viewport": true,
	"binary_file_patterns":
	[
		"node_modules/*",
		"dist/*",
		"deploy/*",
		"build/*",
		"dest/*",
		"*.log",
		"*.min.*",
		"bower_components/*",
		"chromeApp/*",
		".sass-cache/*",
		"tests/*",
		"social/*"
	],
	"bold_folder_labels": true,
	"color_scheme": "Packages/Material Theme/schemes/Material-Theme-Darker.tmTheme",
	"draw_centered": true,
	"enable_tab_scrolling": false,
	"ensure_newline_at_eof_on_save": true,
	"folder_exclude_patterns":
	[
	],
	"font_face": "Hack",
	"font_options":
	[
		"gray_antialias"
	],
	"font_size": 17,
	"gutter": true,
	"highlight_line": true,
	"ignored_packages":
	[
		"Markdown",
		"Vintage"
	],
	"indent_guide_options":
	[
		"draw_normal",
		"draw_active"
	],
	"line_numbers": true,
	"line_padding_bottom": 3,
	"line_padding_top": 3,
	"material_theme_accent_lime": true,
	"material_theme_bold_tab": true,
	"material_theme_compact_sidebar": true,
	"material_theme_contrast_mode": true,
	"material_theme_small_statusbar": true,
	"material_theme_tabs_autowidth": true,
	"material_theme_tabs_separator": true,
	"overlay_scroll_bars": "enabled",
	"remember_full_screen": true,
	"scroll_past_end": true,
	"show_encoding": true,
	"show_full_path": true,
	"spell_check": true,
	"tab_size": 2,
	"theme": "Material-Theme-Darker.sublime-theme",
	"translate_tabs_to_spaces": true,
	"trim_trailing_white_space_on_save": true,
	"word_wrap": true
}

```

### Key Bindings
```js
[{
    "keys": ["super+shift+b"],
    "command": "jsbeautify",
    "context": [{
        "key": "selector",
        "operator": "equal",
        "operand": "source.js,source.json,source.jade"
      }
    ]
  },
  { "keys": ["super+alt+down"], "command": "goto_definition" },
  { "keys": ["super+ctrl+o"], "command": "reveal_in_side_bar" },
  { "keys": ["ctrl+r"], "command": "side_bar_rename" }, //rename file
  { "keys": ["ctrl+shift+m"], "command": "side_bar_move" }, //move file
]
```

### License
@xwartz

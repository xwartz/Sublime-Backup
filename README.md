
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
		"deploy/*",
		"build/*",
		"dest/*",
		"*.log",
		"*.min.*",
		"bower_components/*",
		"template/*.js",
		"chromeApp/*",
		".sass-cache/*",
		"dist/*"
	],
	"bold_folder_labels": true,
	"color_scheme": "Packages/Material Theme/schemes/Material-Theme-Darker.tmTheme",
	"draw_centered": true,
	"enable_tab_scrolling": false,
	"ensure_newline_at_eof_on_save": false,
	"folder_exclude_patterns":
	[
	],
	"font_face": "Hack",
	"font_options":
	[
		"gray_antialias"
	],
	"font_size": 18,
	"gutter": true,
	"highlight_line": true,
	"ignored_packages":
	[
		"Markdown",
		"Vintage"
	],
	"line_numbers": true,
	"line_padding_bottom": 2,
	"line_padding_top": 2,
	"material_theme_accent_yellow": true,
	"material_theme_bold_tab": true,
	"material_theme_small_statusbar": true,
	"overlay_scroll_bars": "enabled",
	"scroll_past_end": true,
	"show_encoding": true,
	"show_full_path": true,
	"tab_size": 2,
	"theme": "Material-Theme-Darker.sublime-theme",
	"translate_tabs_to_spaces": true,
	"trim_trailing_white_space_on_save": false,
	"word_wrap": false
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
  {
  "keys": ["tab"], 
  "command": "expand_abbreviation_by_tab", 
  // put comma-separated syntax selectors for which 
  // you want to expandEmmet abbreviations into "operand" key 
  // instead of SCOPE_SELECTOR.
  // Examples: source.js, text.html - source
  "context": [
    {
      "operand": "meta.group.braces.round.js, text.html", 
      "operator": "equal", 
      "match_all": true, 
      "key": "selector"
    }, 

    // run only if there's no selected text
    {
      "match_all": true, 
      "key": "selection_empty"
    },

    // don't work if there are active tabstops
    {
      "operator": "equal", 
      "operand": false, 
      "match_all": true, 
      "key": "has_next_field"
    }, 

    // don't work if completion popup is visible and you
    // want to insert completion with Tab. If you want to
    // expand Emmet with Tab even if popup is visible -- 
    // remove this section
    {
      "operand": false, 
      "operator": "equal", 
      "match_all": true, 
      "key": "auto_complete_visible"
    }, 
    {
      "match_all": true, 
      "key": "is_abbreviation"
    }
  ]
}
]
```

### License
@xwartz

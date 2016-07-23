# Sublime Config
My Sublime Text configuration and plugins :green_heart:.

![][https://github.com/jordanamorais/sublime-config/blob/master/img/sublime-config.JPG]

## Theme ##

* [Themr](https://packagecontrol.io/packages/Themr) - To manage and select my installed themes.
* [Material-Theme](https://packagecontrol.io/packages/Material%20Theme) - My current favorite theme.
* [Material Theme - App Bar] (https://packagecontrol.io/packages/Material%20Theme%20-%20Appbar) - Tinted appbar to your Material Theme installation :two_hearts:.
If you like to change de App Bar color, just add one of this lines to your Sublime `Preferences: Settings - User`:

``` 
"material_theme_appbar_lime": true,
"material_theme_appbar_orange": true,
"material_theme_appbar_purple": true,
"material_theme_appbar_red": true,
"material_theme_appbar_yellow": true,
"material_theme_appbar_indigo": true,
"material_theme_appbar_pink": true,
"material_theme_appbar_blue": true,
"material_theme_appbar_cyan": true
```

## Plugins ##

#### Files ####
* [AdvancedNewFile] (https://packagecontrol.io/packages/AdvancedNewFile) - Advanced File Creation.
* [SideBarEnhancments] (https://packagecontrol.io/packages/SideBarEnhancements) - Provides enhancements to the operations on Sidebar of Files and Folders.
* [Compare Side-by-side] (https://packagecontrol.io/packages/Compare%20Side-By-Side) - A simple side-by-side comparison tool.

#### Autocomplete ####
* [All Autocomplete] (https://packagecontrol.io/packages/All%20Autocomplete) - Extends the default autocomplete to find matches in all open files.

#### Highlighters ####
* [BracketHighLighter] (https://packagecontrol.io/packages/BracketHighlighter)
* :star2: [Color HighLighter] (https://packagecontrol.io/packages/Color%20Highlighter) - Previews color values by underlaying the selected hex codes in different styles.

#### CSS/SASS and linters ####
* :star2: [Emmet] (https://packagecontrol.io/packages/Emmet) - Greatly improves HTML & CSS workflow.
* :star2: [Sass] (https://packagecontrol.io/packages/Sass)
* [SublimeLinter] (https://packagecontrol.io/packages/SublimeLinter) - Code linting.
* :star2: [SublimeLinter-contrib-scss-lint] (https://packagecontrol.io/packages/SublimeLinter-contrib-scss-lint) - Provides an interface to the [scss-lint] (https://github.com/brigade/scss-lint). It will be used with files that have the “SCSS” syntax.

#### Markdown ####
* :star2: [MarkdownEditing] (https://packagecontrol.io/packages/MarkdownEditing) - Provides a decent Markdown color scheme (light and dark) with more robust syntax highlighting and useful Markdown editing features.
* :star2: [Markdown Preview] (https://packagecontrol.io/packages/Markdown%20Preview) - Preview your Markdown files quickly in your web browser.

#### Git/Github ####
* :star2: [Git] (https://packagecontrol.io/packages/Git) - Provides Git integration.
* [GitHub Tools] (https://packagecontrol.io/packages/Github%20Tools)

#### Template Engines ####
* [Jade] (https://packagecontrol.io/packages/Jade) - Jade template engine. (*:pushpin: Jade has been renamed to Pug*)
* [Bootstrap 3 Jade Snippets] (https://packagecontrol.io/packages/Bootstrap%203%20Jade%20Snippets)

## Code Style ##

#### Soft Tabs ####
I started to use Soft Tabs (tabs with two spaces) instead of Hard Tabs ([See this stackoverflow question] (http://stackoverflow.com/questions/9446109/soft-tabs-or-hard-tabs)). If you want to, add this to your `Sublime Settings - User` Preferences:

``` 
{
    "tab_size": 2,
    "translate_tabs_to_spaces": true
}
```

#### SCSS Lint indentation config ####

In my `default.yml` scss-lint config file, i changed the `Indentation character` to `tab` instead of `spaces`:

```
Indentation:
    ...
    character: tab # or 'spaces'
    width: 1
```

*:pushpin: (TO DO: Remember to "do the right way", creating the `scss-lint.yml` into the current working directory later)*

## Key Bindings ##

My `Key Bindings - User` Preferences also with [eclipse] (https://eclipse.org/) keybindings.

```
[
  { "keys": ["f12"], "command": "htmlprettify"},
  { "keys": ["f1"], "command": "fold" },
  { "keys": ["f2"], "command": "unfold" },
  { "keys": ["ctrl+à"], "command": "show_overlay", "args": {"overlay": "goto", "text": "@"} },
  { "keys": ["ctrl+!"], "command": "show_overlay", "args": {"overlay": "goto", "text": ":"} },
  { "keys": ["ctrl+space"], "command": "auto_complete" },
  { "keys": ["ctrl+space"], "command": "replace_completion_with_auto_complete", "context":
    [
      { "key": "last_command", "operator": "equal", "operand": "insert_best_completion" },
      { "key": "auto_complete_visible", "operator": "equal", "operand": false },
      { "key": "setting.tab_completion", "operator": "equal", "operand": true }
    ]
  },
  { "keys": ["ctrl+d"], "command": "run_macro_file", "args": {"file": "Packages/Default/Delete Line.sublime-macro"} },
  { "keys": ["ctrl+shift+c"], "command": "toggle_comment", "args": { "block": false } },
  { "keys": ["ctrl+shift+c"], "command": "toggle_comment", "args": { "block": true } },
  { "keys": ["ctrl+shift+f"], "command": "reindent" , "args": {"single_line": false}},
  { "keys": ["ctrl+shift+s"], "command": "save_all" },
  { "keys": ["alt+up"], "command": "swap_line_up" },
  { "keys": ["alt+down"], "command": "swap_line_down" },
  { "keys": ["ctrl+alt+j"], "command": "join_lines" },
  { "keys": ["ctrl+alt+down"], "command": "duplicate_line" },
  { "keys": ["shift+ctrl+r"], "command": "show_overlay", "args": {"overlay": "goto", "show_files": true} },
  { "keys": ["shift+ctrl+f4"], "command": "close_all" },
  { "keys": ["shift+ctrl+y"], "command": "lower_case" },
  { "keys": ["shift+ctrl+x"], "command": "upper_case" }
] 
```

[https://github.com/jordanamorais/sublime-config/blob/master/img/sublime-config.JPG]: https://github.com/jordanamorais/sublime-config/blob/master/img/sublime-config.JPG

# Sublime Config
My Sublime Text configuration and plugins :green_heart:.

![][https://github.com/jordanamorais/sublime-config/blob/master/img/sublime-config.JPG]

## Theme ##

* [Themr](https://packagecontrol.io/packages/Themr) - To manage and select my installed themes.
* [Material-Theme](https://packagecontrol.io/packages/Material%20Theme) - My current favorite theme
* [Material Theme - App Bar] (https://packagecontrol.io/packages/Material%20Theme%20-%20Appbar) - Tinted appbar to your Material Theme installation :two_hearts:

## Plugins ##

### Files ###
* [AdvancedNewFile] (https://packagecontrol.io/packages/AdvancedNewFile) - Advanced File Creation.
* [SideBarEnhancments] (https://packagecontrol.io/packages/SideBarEnhancements) - Provides enhancements to the operations on Sidebar of Files and Folders
* [Compare Side-by-side] (https://packagecontrol.io/packages/Compare%20Side-By-Side) - A simple side-by-side comparison tool.

### Autocomplete ###
* [All Autocomplete] (https://packagecontrol.io/packages/All%20Autocomplete) - Extends the default autocomplete to find matches in all open files.

### Highlighters ###
* [BracketHighLighter] (https://packagecontrol.io/packages/BracketHighlighter)
* :stars: [Color HighLighter] (https://packagecontrol.io/packages/Color%20Highlighter) - Previews color values by underlaying the selected hex codes in different styles.

### CSS/SASS and Linters###
* :stars: [Emmet] (https://packagecontrol.io/packages/Emmet) - Greatly improves HTML & CSS workflow.
* [Sass] (https://packagecontrol.io/packages/Sass)
* [SublimeLinter] (https://packagecontrol.io/packages/SublimeLinter) - Code linting.
* :stars: [SublimeLinter-contrib-scss-lint] (https://packagecontrol.io/packages/SublimeLinter-contrib-scss-lint) - Provides an interface to the [scss-lint] (https://github.com/brigade/scss-lint). It will be used with files that have the “SCSS” syntax.

### Markdown ###
* :stars: [MarkdownEditing] (https://packagecontrol.io/packages/MarkdownEditing) - Provides a decent Markdown color scheme (light and dark) with more robust syntax highlighting and useful Markdown editing features.
* :stars: [Markdown Preview] (https://packagecontrol.io/packages/Markdown%20Preview) - Preview your Markdown files quickly in your web browser.

### Git/Github ###
* :stars: [Git] (https://packagecontrol.io/packages/Git) - Provides Git integration.
* [Git Gutter] (https://packagecontrol.io/packages/GitGutter) - Show an icon in the gutter area indicating whether a line has been inserted, modified or deleted.
* [GitHub Tools] (https://packagecontrol.io/packages/Github%20Tools)

### Template Engines ###
* [Jade/Pug] (https://packagecontrol.io/packages/Jade) - Jade/Pug template engine.
* [Bootstrap 3 Jade Snippet] (https://packagecontrol.io/packages/Bootstrap%203%20Jade%20Snippets)

## Code Style ##

### Soft Tabs ###
I started to use Soft Tabs (tabs with two spaces) instead of Hard Tabs ([See this stackoverflow question] (http://stackoverflow.com/questions/9446109/soft-tabs-or-hard-tabs)). If you want to, add this to your Sublime User Preferences:

``` 
{
    "tab_size": 2,
    "translate_tabs_to_spaces": true
}
```

## Key Bindings ##

My User Key Bindings Preferences also with [eclipse] (https://eclipse.org/) keybindings.

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

# ExportHtml

## 1.3.3

- fixed a bug for combinator selectors

## 1.3.2

- Optimized the way, unused css declarations are selected.
- Clean selection/deletion in multiple declarations

## 1.3.1

- fixed a bug for inline css

## 1.3.0

- settings can now be configured over a project specific file "unused_css.cfg" that has to be located in a projects root path
- added 'unused_css_ignore_selectors' setting: Every element in this array will be ignored in the search and never be stated as non occured selector. Can also be defined as id or class selector, e.g. "#example", ".example", "example"
- added 'unused_css_delete_on_search' setting: Every unused css selector that was found during the search will be removed after the search
- switched default behaviour of plugin. Instead of highlighting every unused selector, they will be selected via cursor, to be able to remove them with one backspace press
- added 'unused_css_highlight_selectors' setting: switch to old behaviour, that unused selectors will be highlighted instead of selected via cursor
- added plugin to sublime context menu on right click to be able to configure some settings and also run the command without shortcut
- most of these changes are based on the ideas from NoxNoctis2, thanks for that

## 1.2.2

- optimized the search patterns to only find the exact selector names and no words where they occur as substring

## 1.2.1

- fixed a bug in the plugin default settings file
- added debugging functionality

## 1.2.0

- the plugin now works for inline css as well
- added configuration path into sublime menu: "Preferences/Package Settings/UnusedCssFinder/"
- Added default key bindings to the project

## 1.1.0

- Added settings to define folders, in which the search takes place
- Fixed a bug to truely search asynchronously
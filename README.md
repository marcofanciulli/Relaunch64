Changelog
================

Relaunch64 3.1.0
----------------

### New features
* completely new editor component with new features, such as:
  - increased performance
  - much faster syntax highlighting
  - rectangular text selection (ctrl+mouse)
  - code-folding
  - proper text anti-aliasing
  - improved line number display and handling
  - changes on color scheme, font and tab size etc. immediately take effect
* improved suggestion / auto-completion popup (ctrl+space and ctrl+shift+space):
  - local labels outside the scope are not listed (only global labels and labels within scope)
  - filter suggestion list by typing
  - editor scrolls to suggestion popup when caret is not visible
* added DASM support
* added TMPx support
* added code-folding support
* added alternative syntax highlighting mode (see preferences)
* improvements with goto error functions
* jump to next/prev code fold function
* Aqua Look'n'Feel on OS X by default
* UI font scaling to better fit screen resolution (can be switched off via preferences, not supoorted with Aqua-Look'n'Feel)
* Added apply-button to Other-tab of preference pane
* many (code) improvements, code cleanup

### Bug fixes
* Modified files, which should have been saved before compiling, were not checked if they really exist.

Relaunch64 3.0.1
----------------

### New features
* added support for CA65
* added support for DreamAss
* added ACME macro and math function support (syntax highlighting, auto-completion)
* goto prev/next error also searches inside included files (even not opened files, which will be opened then)
* goto error now scrolls the log to the related line with error description
* auto-completion for functions, macros and scripting commands (ACME, Kick Assembler, 64tass, DreamAss) (press ctrl+shift+space while typing)
* automatic goto error line when compiling errors occur
* last 15 recently used find terms will be stored per session
* improved tab/shift+tab behaviour with selected text
* added quick references (menu view)
* added regular expression checkbox to find-command, to explicitly en-/disable search for regular expressions
* added checkboxes for whole-word and match-case search
* added syntax highlighting for scripting commands (Kick Assembler, 64tass)
* added SOURCEDIR as additional place holder in user scripts
* added "script" comment-command (see help-file)
* added new syntax highlighting color schemes
* more file extensions are now accepted on drag'n'drop
* slight modification of C64 scheme

### Bug fixes
* bug fix with "Jump to label" function with Kick Assembler
* bug fix with "Find next" when content was changed
* bug fix with "Replace" function
* bug fix with auto-indent and unintended insert of new line
* changed auto-completion feature, which did not work with labels with less than 3 chars, and now works for labels with at least 1 char

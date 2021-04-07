# Related Repositories

* https://github.com/hl2guide/Awesome-Visual-Studio-Code-Extensions
* https://github.com/hl2guide/Awesome-Visual-Studio-Code-Keyboard-Shortcuts

# Input

The vast majority of efficient input comes from typing on the keyboard.

Learn the keyboard shortcuts, focusing on the ones that you will use the most using the below Keyboard Reference Sheets.

This guide uses the Windows keyboard shortcuts.

## Keyboard Reference Sheets

These are the official Microsoft PDF files:

* Windows: https://go.microsoft.com/fwlink/?linkid=832145
* Linux: https://go.microsoft.com/fwlink/?linkid=832144
* MacOS: https://go.microsoft.com/fwlink/?linkid=832143

## Quickly Opening Files

To open a file quickly press `Ctrl+P`.

## Opening Recent Files

To open any recently opened file press `Ctrl+R`.

# Configuration

To access the __Settings__ page press `Ctrl+,`.

## Customizing Keyboard Shortcuts

To set your own keyboard shortcuts press `Ctrl+K` then `Ctrl+S`.

## Fonts and Font Ligatures

You can set your own custom font (for any installed font) and whether to use _font ligatures_ or not in the __Settings__ page.

Ligatures make it so things like `!=` `==` and `===` render properly. Fonts __must__ support ligatures for it to take effect.

For all coding I personally recommend using the font Iosevka:
https://github.com/be5invis/Iosevka

Make sure that font installed and appears on an OS level first.

On the settings page use the search bar to search for `Editor: Font Family`.

For the `Editor: Font Family` result type in `Iosevka, sans-serif`.

For the `Terminal › Integrated: Font Family` result type in `Iosevka Term, monospace`.

## Tab Size

On the settings page use the search bar to search for `Editor: Tab Size`.

For the `Editor: Tab Size` result set it to your liking. I recommend `4`.

## Rendering Whitespace

On the settings page use the search bar to search for `Editor: Render Whitespace`.

For the `Editor: Render Whitespace` result set it to your liking. I recommend `all`.

# Editor

## Text Selection

* Your mouse can select text easily in most scenarios.
* Press `Shift+Up` or `Shift+Down` to select lines.

## Multi Cursor Editing

To add cursors at arbitrary positions, select a position with your mouse and use `Alt+Click`.

To set cursors above or below the current position press `Ctrl+Alt+Up` or `Ctrl+Alt+Down`

You can add additional cursors to all occurrences of the current selection by pressing `Ctrl+Shift+L`.

## Fast Scrolling

To fast scroll press and hold `alt` and then press `up` or `down` or use your mouse wheel.

To resume normal scrolling simply release the `alt` key.

## Copy Line Up or Down

To copy and entire line up or down press `Shift+Alt+Up` or `Shift+Alt+Down`.

## Move Line Up or Down

To move and entire line up or down press `Alt+Up` or `Alt+Down`.

## Navigating to a Line

Press `Ctrl+G`, type in a line number and press `Enter` to go a specific line.

## Selecting a Line

Press `Ctrl+L` to select the current line that the cursor is at.

## Deleting a Line

Press `Ctrl+Shift+K` to delete and entire line.

## Formatting a Selection

Select a section of code and then press `Ctrl+K` then `Ctrl+F` to format selected text.

Press `Shift+Alt+F` to format an entire document.

## Code Folding

When working with a large document folding (collapsing) sections of code is really useful to focus on a particular section.

* Press `Ctrl+Shift+[` to fold selected lines.
* Press `Ctrl+Shift+]` to unfolder selected lines.
* Press `Ctrl+K` then `Ctrl+0` to fold all sections in a document.
* Press `Ctrl+K` then `Ctrl+J` to unfold all sections in a document.

## Errors and Warnings

Press `Ctrl+Shift+M` to view errors and warnings for the current document, depending on the type of document.

## IntelliSense

For documents that support IntelliSense you can use `Ctrl+Space` while coding to get suggestions for method names, parameters etc.

## Find

To find a string within the current document:

* Press `Ctrl+F`
* Type in the search string
* Press `Enter` to jump to the first result found

## Find and Replace

To replace one or all occurences of a string within the current document:

* Press `Ctrl+H`
* In the __first__ field type in the string to find
* In the __second__ field type in the string to replace with
* Press `Enter` to perform one replacement __OR__ `Ctrl+Alt+Enter` to replace all occurences

### Regular Expression Replaces

Regular expressions are powerful and allow for:

* Prefixing
* Suffixing
* Pattern Matching

While the replace dialog is active press `Alt+R` to toggle regular expressions on or off.

#### Prefixing

To add a string to the beginning of each line.

Note: `(.*)` means "zero or more characters" and `$1` means "the entire line".

E.g. to prefix `TEXT-`:

* Press `Ctrl+H`
* In the __first__ field type in `(.*)`
* In the __second__ field type in the string `TEXT-$1`
* Press `Enter` to perform one replacement __OR__ `Ctrl+Alt+Enter` to replace all occurences

#### Suffixing

To add a string to the end of each line.

Note: `(.*)` means "zero or more characters" and `$1` means "the entire line".

E.g. to suffix `.zip`:

* Press `Ctrl+H`
* In the __first__ field type in `(.*)`
* In the __second__ field type in the string `$1.zip`
* Press `Enter` to perform one replacement __OR__ `Ctrl+Alt+Enter` to replace all occurences

#### Pattern Matching

Note: `(.*)` means "zero or more characters".

To replace all lines that contain `A1` with `paper`:
* Press `Ctrl+H`
* In the __first__ field type in `(.*)A1(.*)`
* In the __second__ field type in the string `paper`
* Press `Enter` to perform one replacement __OR__ `Ctrl+Alt+Enter` to replace all occurences

For more info on the power of regular expressions please refer to: [Use regular expressions in Visual Studio](https://docs.microsoft.com/en-us/visualstudio/ide/using-regular-expressions-in-visual-studio?view=vs-2019)

__Have fun!__

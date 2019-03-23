# Vim

## Insert mode
  ctrl - r: Insert registers
  ctrl - a: Repeat last insert

  ctrl - p/n: Autocomplete previous or next instances

  ctrl - ]: Go to word definition

  ctrl - x: Special insertion mode
    ctrl - ]: Insert from word definition (tag completion)
    ctrl - f: Autocompletion from file names
    ctrl - p/n: Context-aware word completion
    ctrl - l: Context-aware line completion
    ctrl - o: Language completion

## Command mode
  ctrl - o/i: Toggle between tags

## Shai
Update: Sublime Text is now my main editor. When I use vim, I use with it with the default keymap. No further updates are planned for colemak.vim

I'm a big fan of the Vim editor, and it is also great for ergonomic reasons. For a very long time I've been working on a completely redesigned keyboard mapping for Vim.

Some of the features:
* The navigation with it is much more intuitive and comfortable, using the IJKL keys (QWERTY), instead of the classic HJKL.
* Turbo navigation: holding the shift key while pressing the IJKL keys (QWERTY) is like pressing five times the key. It's really comfortable once you get used to it.
* Navigation in insert mode: holding the Ctrl key while pressing UIOK (QWERTY) is like the arrow keys.
* Easy word navigation using U/O/P keys (QWERTY).
* Easy PageUp/PageDown using the Y/H keys (QWERTY).
* The undo/cut/yank (copy)/paste correspond to the ZXCV keys.
* Tab replaces Escape to switch back to command mode (press Shift+Tab for a normal Tab).
* Visual mode/Replace/Insert/Append are are all in the home position on the ASDF keys (QWERTY).
* (GUI only) Intuitive support for tabs, Ctrl+T opens a new tab, Ctrl+W closes tabs. Ctrl+Tab switches tabs.
* (GUI only) Quick line reordering (holding Ctrl+Shift+up/down).
* Easy cursor history using ( and ).
* Whitespace/deletion keys work in both insert and command modes.
* Easy macro record and playback (qq to start recording, q to end recording, Q to playback)
* Easy line jumping (- key)
* Easy indention using Space/Shift+Space/Shift+Tab in visual line/block mode.
* Insert/Add also work in Visual Line mode like they work in Visual Block mode.
* : commands can be typed using a ; without holding shift (e.g. :wq can be typed as ;wq)
* (GUI only) Ctrl+C/Ctrl+V can copy and paste on the command line (selection must be done with the mouse)
* (GUI only) Ctrl+C/Ctrl+X copy/cut the current line if nothing is selected

I've been using it for the last few months and I'm very happy with it, but it should still be considered experimental. The documentation is embedded inside the Vim file, so it might take a little while to figure things out. That said, it is much more intuitive than the Vim mapping.

It is _very_ different from the normal Vim and it will take some time to used to it. There is some functionality that had to be sacrificed.

Download colemak.vim (experimental, requires Vim 7.0 or later, gVim recommended)

It would be great if someone would be able to create a graphical cheat sheet/tutorial for colemak.vim like this one

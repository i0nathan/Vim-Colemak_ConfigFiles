# Vim-Colemak_ConfigFiles
* This layout is taken from Shai and modifications made from jooize and tried to be applies to different vim tools  (browser navigators and packages built for text editors). I hope is clear and useful.

## Layout from [jooize](https://github.com/jooize/vim-colemak#key-mappings)
Colemak layout:                  |                 QWERTY layout:
`12345 67890-=     Move around:  |  (instead of)   `12345 67890-=
 qwfpg jluy;[]\         e        |       k          qwert yuiop[]\
 arstd HNEIo'         h   i      |     h   l        asdfg HJKL;'
 zxcvb km,./            n        |       j          zxcvb nm,./

(  novx)  h = h (Left)     i = l (Right)     e = k (Up)     n = j (Down)

(  novx)  l = b (Back word)            L = B (Back WORD)
(  novx)  y = w (Forward word)         Y = W (Forward WORD)
(  novx)  u = e (Forward end of word)  U = E (Forward end of WORD)

(c     )  <C-L> = <C-Left> (Back WORD)
(c     )  <C-Y> = <C-Right> (Seems to equal forward WORD minus 1 character)

(  n  x)  a = v (Visual)   A = V (Visual line)
(  n   )  r = r (Replace)  R = R (Replace)
(  n   )  s = i (Insert)   S = I (Insert before first non-blank of line)
(  n   )  t = a (Append)   T = A (Append at end of line)
(  n   )  w = c (Change)   W = C (Change to end of line)  ww = cc (Change line)

(  n  x)  z = u (Undo)    Z = <C-R> (Redo)  gz = U (Undo all latest changes on line)
(  n  x)  x = x (Cut)     X = dd (Cut line)
(  n  x)  c = y (Copy)    C = yy (Copy line)
(  n  x)  v = p (Paste)   V = P (Paste)
(  n  x)  gv = gp (Paste) gV = gP (Paste)

(   o  )  r = i (Example: dip -> drp (Delete inner paragraph))

(  no x)  p = t{char} (Before next {char})  P = T{char} (After previous {char})
(  no x)  b = ; (Repeat latest f or t)  B = , (Repeat latest f or t reversed)
(  no x)  k = n (Repeat latest / or ?)  K = N (Repeat latest / or ? reversed)

(  n  x)  j = z
(  n  x)  jn = zj (Next fold) [Also jj = zj]
(  n  x)  je = zk (Previous fold) [Also jk = zk]

(  n   )  ga = gv (Reselect last visual selection)
(  n  x)  gK = K (Lookup)
(  n  x)  gL = L (To line [count] from bottom of window)

(  n  x)  <C-W>h = <C-W>h (Window left)
(  n  x)  <C-W>n = <C-W>j (Window down)
(  n  x)  <C-W>e = <C-W>k (Window up)
(  n  x)  <C-W>i = <C-W>l (Window right)

Lost:
(  n  x)  H (To line [count] from top of window)
(  n  x)  s (Substitute [count] characters) [Use wi = cl]
(  n  x)  S (Substitute [count] lines) [Use ww = cc]
(  n  x)  X (Cut [count] characters backwards) [Use dh = dh]
(  n   )  Z (Quit)
(  n  x)  <C-W>n (Window down) [Use <C-W><C-N> = <C-W><C-N>]
(  n  x)  <C-W>i (Window down) [Use <C-W><C-I> = <C-W><C-I>]

Legend:
<C-X>     Ctrl-X
(c     )  Command-line mode
( i    )  Insert mode
(  n   )  Normal mode
(   o  )  Operator pending
(    v )  Visual+Select mode
(     x)  Visual mode

## Notes about Insert mode
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

## Notes about Command mode
  ctrl - o/i: Toggle between tags

## Notes from (Shai)[https://forum.colemak.com/topic/50-colemak-vim/]
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

# base16-cmus

## Info

Base16 for the cmus theme format. Relies on your terminal colors also being the same so
make sure to use this in conjuction with [base16-xresources] or [base16-iterm2] or
whatever is the right template for the terminal emulator you have.

[base16-xresources]: https://github.com/chriskempson/base16-xresources
[base16-iterm2]: https://github.com/martinlindhe/base16-iterm2

Cmus color display is a little borked, so the terminal colors from 8-15 aren't actually
taken from the terminal color pallete, they are just bold/brighter (depending on terminal
emulator) versions of 0-7. You can see the relevant source code [here]. This doesn't
affect any of the themes here because they only use terminal colors up to 7 (you don't need
that many different colors for the UI of a music program).

Since this template only uses the first 16 ANSI colors, it doesn't even need to be
generated. You can grab [default.mustache](templates/default.mustache) and use it as
your permanent cmus theme. It will always adapt to your terminal colors, whether they
were generated from base16 or not.

[here]: https://github.com/cmus/cmus/blob/d1290d50f9f7585c43b9e1326c0d6d1e0b4583f6/ui_curses.c#L1780

## Install

Put into `~/.config/cmus`.

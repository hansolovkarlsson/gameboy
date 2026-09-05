# Changelog

*The one page that says **when**, for a reader who is not reading the source.
Only what shipped and is visible from outside: a flag that appeared, a
behaviour that changed, a test ROM that now passes, a message somebody will now
see. Internal reworking, and the reasoning behind any of it, belongs in [the
journal](work-journal/) instead.*

The emulator has no version numbers. Entries are grouped by the day the work
happened, newest first, and this page starts from the day it was created — for
what came before it, [GAMEBOY_ROADMAP.md](GAMEBOY_ROADMAP.md)'s `Status`
section records each phase as it landed.

## 2026-09-04

- `make test` now runs the ROM-independent unit suite, as an alias for
  `make gameboy-test`. The ROM-based regressions (`gameboy-visual-test` and the
  byte-exact game targets) keep their own individual names and are not folded
  in — they are slower, and they are the ones worth invoking singly when one of
  them is what you are chasing.

emms-player-mpv.el --- mpv support for EMMS
===========================================

[![MELPA](http://melpa.org/packages/emms-player-mpv-badge.svg)](http://melpa.org/#/emms-player-mpv)
[![MELPA Stable](http://stable.melpa.org/packages/emms-player-mpv-badge.svg)](http://stable.melpa.org/#/emms-player-mpv)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/dochang/emms-player-mpv.svg)](http://isitmaintained.com/project/dochang/emms-player-mpv "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/dochang/emms-player-mpv.svg)](http://isitmaintained.com/project/dochang/emms-player-mpv "Percentage of issues still open")

This library provides a player that uses [mpv] for [EMMS].  It
supports pause and seeking.  For loading subtitles automatically, try
adding `autosub-match=fuzzy` to your `~/.mpv/config`, see mpv manual
for more.

This library is based on `emms-player-mplayer.el' in EMMS.

[mpv]: http://mpv.io/
[EMMS]: https://www.gnu.org/software/emms/

Installation
------------

This library is available on MELPA and el-get as `emms-player-mpv`.

Otherwise, download `emms-player-mpv.el` and put it in your load path.

Usage
-----

Add the following into your `.emacs`:

``` elisp
(require 'emms-player-mpv)
(add-to-list 'emms-player-list 'emms-player-mpv)
```

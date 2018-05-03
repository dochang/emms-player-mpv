WARNING
=======

This package has been merged into [EMMS].  It'll be deprecated and removed from MELPA and el-get.

How to migrate
--------------

 1. Delete this package from Emacs.
 2. You don't need `(require 'emms-player-mpv)` any more, `(require 'emms)` will do that for you.
 3. EMMS has put mpv in its default player list, but you can still customize `emms-player-list`.

NOTE
----

This project won't accept bug reports, feature requests or any other issues any more.  Please send them to [the EMMS mailing list][1].

[1]: https://lists.gnu.org/mailman/listinfo/emms-help

emms-player-mpv.el --- mpv support for EMMS
===========================================

[![MELPA](http://melpa.org/packages/emms-player-mpv-badge.svg)](http://melpa.org/#/emms-player-mpv)
[![MELPA Stable](http://stable.melpa.org/packages/emms-player-mpv-badge.svg)](http://stable.melpa.org/#/emms-player-mpv)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/dochang/emms-player-mpv.svg)](http://isitmaintained.com/project/dochang/emms-player-mpv "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/dochang/emms-player-mpv.svg)](http://isitmaintained.com/project/dochang/emms-player-mpv "Percentage of issues still open")

This library provides a player that uses [mpv] for [EMMS].  It supports pause
and seeking.  See mpv manual for more.

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

FAQ
---

### Loading Subtitles Automatically ###

Put `sub-auto=fuzzy` in your config file.

### Disable GUI Windows when Playing Audio Files ###

Some people want to display image attachments for audios but some people don't.
I decide to leave this config as default.

By default, mpv displays image attachments.  To disable it, put
`audio-display=no` in your config file.

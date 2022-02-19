WARNING
========
Experimental in-progress work.  PROVIDED "AS IS", WITHOUT WARRANTY
OF ANY KIND, EXPRESS OR IMPLIED, see GNU General Public License, version 2
for detailed disclaimer:
https://www.gnu.org/licenses/old-licenses/gpl-2.0.html

Use at your own risk, In the best case you will lose time/work and/or
corrupt your files.

xah-fly-keys-hyper
===================
This is an attempt to rewrite xah-fly-keys to model the command mode state as
a sticky Hyper key.  This makes it easier to define custom key bindings that
depend on xah-fly's command mode state.

E.g.  to create a binding for the command-mode state that is only active in
VHDL mode, we can now add a key binding like

```
  (define-key vhdl-mode-map (kbd "H-SPC v h p") 'vhdl-port-paste-instance)
```

(where "H-" denotes the hyper modifier that is only present in command mode)

Note how this is similar in spirit to Chris Done's god-mode.el .

xah-fly-keys
===================

A modal keybinding for emacs (like vim), but based on command frequency and ergonomics.

This is the most efficient editing system in the universe.

home page at
http://ergoemacs.org/misc/ergoemacs_vi_mode.html

2020-04-18 News: Key Engine Rewrite
===================

Major key engine rewrite by Dan Langlois (https://github.com/DanLanglois) and Will Dey (https://github.com/wi11dey) .

The old stable version is available at
http://ergoemacs.org/misc/i/xah-fly-keys_old_2020-04-18.el

QWERTY layout
-------------------
![xah-fly-keys qwerty layout](xah_fly_keys_qwerty_layout_2020-04-18_4fgyk.png)

Documentation
-------------------

Add the following to `.emacs` after installing manually or via MELPA:
```elisp
(require 'xah-fly-keys)
(xah-fly-keys-set-layout "qwerty") ; required
```

The following keyboard layouts are supported:

* "azerty"
* "azerty-be"
* "colemak"
* "colemak-mod-dh"
* "colemak-mod-dh-new"
* "dvorak"
* "programer-dvorak"
* "qwerty"
* "qwerty-abnt"
* "qwertz"
* "workman"
* "norman"
* ["neo2"](https://neo-layout.org/)
* "koy"
* "adnw"
* "pt-nativo"
* "carpalx-qgmlwy"
* "carpalx-qgmlwb"
* "carpalx-qfmlwy"

Full Documentation
-------------------

http://ergoemacs.org/misc/ergoemacs_vi_mode.html

Been working on this since 2013, and since 2007 on ergoemacs-mode.

Put in 5 bucks in my patreon.
https://www.patreon.com/xahlee

or https://paypal.com
pay to xah@xahlee.org

Thanks.

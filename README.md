# EMMS settings

## Comment

Currently a file with my EMMS streams.

## Installation

1. Install a player, e.g. `mpv`:
``` bash
$ sudo pacman -S mpv
```

2. Setup EMMS for Emacs with `emms-streams` by loading `emms` in your `init.el` like:
``` lisp
(leaf emms

    :ensure t

    :init

    (emms-all)
    (emms-default-players)

    :config

    (leaf emms-streams))
```

3. Create a symbolic link:
```bash
$ ln -s ./streams.emms ~/.emacs.d/emms/streams.emms
```

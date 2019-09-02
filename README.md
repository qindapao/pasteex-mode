# What's this?
It's an Emacs extension, with it you can just use one key to save clipboard image to disk file, and at the same time insert the file link(org-mode/markdown-mode) or file path(other mode) to current point.

Based on the ability of PasteEx, only support Windows platform.

# Prerequisite
- [PasteEx](https://github.com/huiyadanli/PasteEx/releases)

# Installation
Put `pasteex-mode.el` to your `load-path`. The `load-path` is usually `~/elisp/`. It's set in your `~/.emacs` file like this:

```emacs-lisp
(add-to-list 'load-path (expand-file-name "~/elisp"))
(require 'pasteex-mode)
```

# Usage
- Set `PasteEx.exe` executable file path to environment PATH, or set the variable `pasteex-executable-path` in your config file, like this:

```emacs-lisp
(setq pasteex-executable-path "D:/program/PasteEx/PasteEx.exe")
```

- Bind your favority key to function `pasteex-image`, like this:

```emacs-lisp
(define-key pasteex-mode-map (kbd "C-c i") 'pasteex-image)
```

- After you make a screenshot to clipboard, or copy a PNG image file to clipboard, then just press `C-c i` shortcut, and the file link or path will be inserted to your buffer immediately, the screenshot image file is saved to `./img/` directory by default. 

# Tips
- Only support Windows platform, because PasteEx only support Windows now.
- That's all, enjoy it ;)
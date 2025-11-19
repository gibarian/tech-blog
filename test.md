> [!IMPORTANT]
> To set up shell integration (key bindings and fuzzy completion),
> see [the instructions below](#setting-up-shell-integration).

[![Packaging status](https://repology.org/badge/vertical-allrepos/fzf.svg?columns=3)](https://repology.org/project/fzf/versions)

> [!NOTE]
> You can override the default behavior
> * Either by setting `$FZF_DEFAULT_COMMAND` to a command that generates the desired list
> * Or by setting `--walker`, `--walker-root`, and `--walker-skip` options in `$FZF_DEFAULT_OPTS`

> [!WARNING]
> A more robust solution would be to use `xargs` but we've presented
> the above as it's easier to grasp
> ```sh
> fzf --print0 | xargs -0 -o vim
> ```

---

* [Installation](#installation)
    * [Using Homebrew](#using-homebrew)
    * [Linux packages](#linux-packages)
    * [Windows packages](#windows-packages)
    * [Using git](#using-git)
    * [Binary releases](#binary-releases)
    * [Setting up shell integration](#setting-up-shell-integration)


---


<!-- vim-markdown-toc GFM -->

* [Installation](#installation)
    * [Using Homebrew](#using-homebrew)
    * [Linux packages](#linux-packages)
    * [Windows packages](#windows-packages)
    * [Using git](#using-git)
    * [Binary releases](#binary-releases)
    * [Setting up shell integration](#setting-up-shell-integration)

<!-- vim-markdown-toc -->



> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
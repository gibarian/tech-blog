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
---
title: '- Tmux'
---

## config file

```bash title="~/.tmux.conf or /etc/tmux.conf" linenums="1"
# Set scrollback buffer to 50000 lines
set-option -g history-limit 50000

# Status bar always visible
set-option -g status on

# Status bar style (colors can be adjusted to match screen's)
set-option -g status-style "bg=black,fg=white"

# Left side: window list with active window highlighted
set-option -g status-left-length 100
set-option -g status-left '#[fg=white,bg=black]#[default]'

# Right side: hostname, date, and time
set-option -g status-right-length 100
set-option -g status-right '#[fg=white]@#H - %a %d %b - %H:%M'

# Window status format
setw -g window-status-format '#[fg=white]#I #W'
setw -g window-status-current-format '#[fg=black,bg=white]#I #W'
```

## commands 

```bash
tmux list-commands                          # commands list with short help

tmux new-session -s <session_name>          # new session with  name
tmux new -s <session_name>                  # new session with  name

tmux attach-session -t <target_session>     # attach to session with defined name/number
tmux attach -t <target_session>             # attach to session with defined name/number
tmux a -t <target_session>                  # attach to session with defined name/number

tmux detach-client -s <target_session>      # detach client with defined target_session
tmux detach-client -t <target_client>       # detach client with defined target_client
tmux detach [-t ...] [-s ...]               # same but shorter
tmux detach                                 # deatach last session

tmux ls                                     # list sessions
tmux kill-session -t <target_session>       # kill session with defined name/number
```
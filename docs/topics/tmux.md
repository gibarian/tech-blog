---
title: '- Tmux'
---

## commands 

commands list with short help
```bash
tmux list-commands
```

new session with  name
```bash
tmux new-session -s <session_name>
tmux new -s <session_name> 
```

attach to session with defined name/number
```bash
tmux attach-session -t <target_session> 
tmux attach -t <target_session>
tmux a -t <target_session>
```

detach client with defined target_session
```bash
tmux detach-client -s <target_session>
tmux detach-client -t <target_client>
tmux detach [-t ...] [-s ...]
tmux detach
```

list sessions
```bash
tmux ls
```

kill session with defined name/number
```bash
tmux kill-session -t <target_session>
```

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

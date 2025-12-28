---
title: '- Tmux'
---

## config file

```bash title="~/.tmux.conf || /etc/tmux.conf" linenums="1"
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
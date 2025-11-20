| **Shortcut**      | **Description**    |
|-------------------|--------------------|
| alt + a           | Broadcast all      |
| alt + g           | Broadcast to group |
| ctrl + shift + o  | Split horizontally |
| ctrl + shift + e  | Split vertically   |
| ctrl + shift + x  | maximazied current |
| shift + super + g | Ungroup_tab        |

---

```ini linenums="1"
[global_config]
  enabled_plugins = LaunchpadCodeURLHandler, APTURLHandler, Logger, LaunchpadBugURLHandler
  inactive_color_offset = 1.0
  scroll_tabbar = True
  title_inactive_bg_color = "#888a85"
  title_receive_bg_color = "#3465a4"
  title_transmit_bg_color = "#467277"
  window_state = maximise
[keybindings]
  close_term = None
  close_window = None
  next_tab = <Primary>Right
  prev_tab = <Primary>Left
[layouts]
  [[default]]
    [[[child1]]]
      parent = window0
      profile = default
      type = Terminal
    [[[window0]]]
      parent = ""
      type = Window
[plugins]
[profiles]
  [[default]]
    background_color = "#002b36"
    background_darkness = 0.8
    cursor_color = "#aaaaaa"
    font = Inconsolata Medium 10
    foreground_color = "#f3f3f3"
    palette = "#000000:#cc0000:#4e9a06:#c4a000:#3465a4:#75507b:#06989a:#d3d7cf:#555753:#ef2929:#8ae234:#fce94f:#729fcf:#ad7fa8:#34e2e2:#eeeeec"
    scrollback_lines = 50000
    use_system_font = False
  [[default - bright]]
    background_color = "#eeeeec"
    cursor_color = "#eeeeec"
    font = Inconsolata Medium 10
    foreground_color = "#000000"
    palette = "#000000:#cc0000:#4e9a06:#c4a000:#3465a4:#75507b:#06989a:#555753:#555753:#ef2929:#4e9a06:#c4a000:#204a87:#ad7fa8:#3465a4:#555753"
    use_system_font = False
  [[default - dark]]
    cursor_color = "#aaaaaa"
    font = Inconsolata Medium 10
    foreground_color = "#ffffff"
    use_system_font = False
  [[default - nice]]
    background_color = "#002b36"
    background_darkness = 0.8
    cursor_color = "#aaaaaa"
    font = Inconsolata Medium 10
    foreground_color = "#f3f3f3"
    palette = "#000000:#cc0000:#4e9a06:#c4a000:#3465a4:#75507b:#06989a:#d3d7cf:#555753:#ef2929:#8ae234:#fce94f:#729fcf:#ad7fa8:#34e2e2:#eeeeec"
    scrollback_lines = 50000
    use_system_font = False
```
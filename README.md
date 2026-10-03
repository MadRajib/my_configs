# my_configs
Configs/Alias/scripts for my workflow

## TMUX

### Alias & Functions
```bash
# tmuxn <session name>
tmuxn() {
    tmux new-session -A -s "$1"
}

# tmuxk <session name>
tmuxk() {
    tmux kill-session -t "$1"
}

# tmuxl -> list all sessions
tmuxl() {
    tmux ls
}

# tmuxa <session name>
tmuxa() {
    tmux attach -t "$1"
}
```

### Shortcuts

Sessions: 

1. `Ctrl+b s`	-> Choose a session from the session list
1. `Ctrl+b (`	-> Switch to the previous session
1. `Ctrl+b )`	-> Switch to the next session
1. `Ctrl+b d`	-> Detach from the current session

Windows:
1. `Ctrl+b c`   -> Create new window
1. `Ctrl+b ,`	-> Rename current window
1. `Ctrl+b &`	-> Kill current window
1. `Ctrl+b n`	-> Next window
1. `Ctrl+b p`	-> Previous window
1. `Ctrl+b 0-9` -> Switch to window by number

Panes:
1. `Ctrl+b %`	-> Split pane vertically
1. `Ctrl+b "`	-> Split pane horizontally
1. `Ctrl+b x`	-> Kill current pane
1. `Ctrl+b o`	-> Cycle panes
1. `Ctrl+b q`	-> Show pane numbers
1. `Ctrl+b ;`	-> Toggle last active pane
1. `Ctrl+b z`   -> Zoom/unzoom pane

Pane Navigantion:
1. `Ctrl+b ←/→/↑/↓`	     -> Move between panes
1. `Ctrl+b Ctrl+←/→/↑/↓` ->	Resize the current pane
1. `Ctrl+b Alt+1`        -> Select the even-horizontal layout
1. `Ctrl+b Alt+2`	     -> Select the even-vertical layout
1. `Ctrl+b Alt+5`	     -> Select the tiled layout

Copy Mode
1. `Ctrl+b [`	-> Enter copy mode
1. `q`	        -> Exit copy mode
1. `Space`  	-> Start selection
1. `Enter`	    -> Copy selection
1. `Ctrl+b ]`	-> Paste buffer
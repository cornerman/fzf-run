# fzf-run

Program launcher based on fzf and dmenu_path.


## Usage

Inside the current terminal:

```
fzf-run
```

Launch a terminal with it (e.g. alacritty):
```
alacritty --option font.size=20 -e fzf-run
```

Example usage with i3 for your `~/.i3/config`:
```
bindsym --release $mod+d exec --no-startup-id alacritty --option font.size=20 -t alacritty-fzf-run -e fzf-run
for_window [title="alacritty-fzf-run"] floating enable, resize set 1500 px 2000 px; move position center; exec --no-startup-id xdotool search --title alacritty-fzf-run behave %@ blur windowclose
```

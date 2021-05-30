# Getting Started with Putty and Byobu
1) Refer to https://www.naturalborncoder.com/linux/2014/10/28/getting-started-with-byobu/ for the setting of putty (or putty tray) and byobu. <br>
To enable the function keys under “Terminal > Keyboard > The Function keys and keypad” select “Xterm R6”. I still keep setting select “Connection > Data > Terminal-type string” as "xterm". <br>
The ”Fn“ key and "Alt" key can work properly when I use byobu through putty/ssh. <br>
2) Unfortunately, the "Ctrl" key and "Shift" key don't work for me in byobu. As a walkarund, I change the file  `f-keys.tmux` under `/usr/share/byobu/keybindings` like below. Then I can mostly use "Alt" key and "Fn" key to do what I want. <br>
	#Note: I use "Alt+F1" to do horizontal split: <br>
	**bind-key -n M-F1 display-panes \; split-window -h -c "#{pane_current_path}"** <br>
	#Note by begood: I use "Alt+F2" to do vertical split: <br>
	**bind-key -n M-F2 display-panes \; split-window -v -c "#{pane_current_path}"** <br>

	#Note: I use vim manner "Alt+jkhl" to select different pane: <br>
	**bind-key -n M-k display-panes \; select-pane -U <br>
	bind-key -n M-j display-panes \; select-pane -D <br>
	bind-key -n M-h display-panes \; select-pane -L <br>
	bind-key -n M-l display-panes \; select-pane -R** <br>

	#Note: I use vim manner again "Ctrl+Alt+jkhl" to resize different pane: <br>
	**bind-key -n C-M-k resize-pane -U <br>
	bind-key -n C-M-j resize-pane -D <br>
	bind-key -n C-M-h resize-pane -L <br>
	bind-key -n C-M-l resize-pane -R** <br>


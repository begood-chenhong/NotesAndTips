# Getting Started with Putty and Byobu
1) Refer to https://www.naturalborncoder.com/linux/2014/10/28/getting-started-with-byobu/ for the setting of putty (or putty tray) and byobu.  To enable the function keys under “Terminal > Keyboard > The Function keys and keypad” select “Xterm R6”. I still keep setting select “Connection > Data > Terminal-type string” as "xterm".
The ”Fn“ key and "Alt" key can work properly when I use byobu through putty/ssh.
2) Unfortunately, the "Ctrl" key and "Shift" key don't work for me in byobu. As a walkarund, I change the file  `f-keys.tmux` under `/usr/share/byobu/keybindings` like below. Then I can mostly use "Alt" key and "Fn" key to do what I want.
#Note: I use "Alt+F1" to do horizontal split:  
**bind-key -n M-F1 display-panes \; split-window -h -c "#{pane_current_path}"**  
#Note by begood: I use "Alt+F2" to do vertical split:  
**bind-key -n M-F2 display-panes \; split-window -v -c "#{pane_current_path}"**  

	#Note by begood: I use vim manner "Alt+jkhl" to select different pane:  
	**bind-key -n M-k display-panes \; select-pane -U  
	bind-key -n M-j display-panes \; select-pane -D  
	bind-key -n M-h display-panes \; select-pane -L  
	bind-key -n M-l display-panes \; select-pane -R**  

	#Note by begood: I use vim manner again "Ctrl+Alt+jkhl" to resize different pane:  
	**bind-key -n C-M-k resize-pane -U  
	bind-key -n C-M-j resize-pane -D  
	bind-key -n C-M-h resize-pane -L  
	bind-key -n C-M-l resize-pane -R**  



> Written with [StackEdit](https://stackedit.io/).

# bspgh0st-Parrot_OS
Install bspwm sxhkd rofi polybar Parrot OS

![bspwm](https://user-images.githubusercontent.com/94316140/221245910-3c3178ec-623b-4331-b429-1a48a4a7ef2a.png)

# Install BSPWM
git clone https://github.com/R3D-GHOST/bspgh0st-Parrot_OS.git


cd bspgh0st-Parrot_OS/


python3 bspghost.py


# SXHKD 


 terminal emulator
super + Return
	kitty 

 program launcher
super + d
	bash ~/.config/polybar/pwidgets/scripts/launcher.sh 

 make sxhkd reload its configuration files:
super + Escape
	pkill -USR1 -x sxhkd


bspwm hotkeys

 quit/restart bspwm
super + alt + {q,r}
	bspc {quit,wm -r}

 close and kill
super + {_,shift + }w
	bspc node -{c,k}

 alternate between the tiled and monocle layout
super + m
	bspc desktop -l next

 send the newest marked node to the newest preselected node
super + y
	bspc node newest.marked.local -n newest.!automatic.local

 swap the current node and the biggest window
super + g
	bspc node -s biggest.window


 state/flags

 set the window state
super + {t,shift + t,s,f}
	bspc node -t {tiled,pseudo_tiled,floating,fullscreen}

 focus/swap

 focus the node in the given direction
super + shift + {Left,Down,Up,Right}
	bspc node -{f,s} {west,south,north,east}

 move/resize

 move a floating window
super + {Left,Down,Up,Right}
	bspc node -v {-20 0,0 20,0 -20,20 0}



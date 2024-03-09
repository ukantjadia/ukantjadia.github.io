---
title: Learn Termux a Terminal Multiplexer
subtitle: "Learn the best tool you can have on a non-GUI server or machine."
summary: "Learn the best tool you can have on a non-GUI server or machine."


draft: false
date: 2023-12-30T14:22:29+05:30
lastmod: 

categories:
    - Uniux
    - Tool
tags:
    - Linux
    - tmux
    - Terminal


projects: []
featured: false
# authors:
#   - Ukant Jadia
image:
  caption: ''
  focal_point: ''
  placement: 2
  preview_only: false

---
# tmux

<!-- ---
## bullet point 
1. install 
2. what it is
3. what it can do 
4. tmux key binding
5. tmux conf
6. extra features 
7. patching for history backups 
8. 
---
### data 💽 -->
## Installation

+ Linux : ``sudo apt-get install tmux``
+ Fedora : ``sudo dnf -y install tmux``
+ Cent-OS : ``sudo yum -y install tmux``
+ Arch Linux : `sudo pacman -S tmux`
+ to start : `tmux`
+ NOTE: Prefix key : `Ctrl+b`
+ [github](https://github.com/tmux/tmux)

## What is tmux ??

+ It is terminal multiplexer.
+ It acts as a window manager in your terminal.
+ It also allows to create multiple window and panes in a single terminal window.

## What it can do

+ Tmux keeps the sessions , windows and panes in a server located at `/tmp/tmux`
+ If your terminal window is crash or killed(*detach*) then still all your process and session is alive, until you kill the tmux server(reboot).
+ Again you can pick the session from where you left by simply *attaching* to the session.
+ tmux is also helpful while working with remote machine.

## tmux key binds

 NOTE: Prefix key `C-b` == `Ctrl+b`

+ to start : `tmux`
+ Splitting Pane :
 	+ for left and right : `C-b+%`
 	+ for top and bottom : `C-b+"`
+ Navigates through panes :
 	+ `C-b+<arrow_keys`
 	+ to move left : `C-b ⬅`
 	+ to move right : `C-b ➡`
 	+ to move up : `C-b ⬆`
 	+ to move down : `C-b ⬇`
+ Closing pane:  type `exit` or `C-b x`
+ Creating windows : `C-b c`
 	+ rename windows : `C-b ,`
 	+ to kill window : `C-b &`
+ Navigates through windows :
 	+ for previous window :  `C-b p`
 	+ for next window :  `C-b n`
 	+ for required : `C-b <number>`
  where number is number in front of the window's name in your status bar
+ Session handling :
 	+ to detach your current session : `C-b d`
  + for list of session to detach : `C-b D`
 	+ for list of session : `C-b s`
 	+ for list of session : `tmux ls`  it worked without a tmux session
 	+ to attach to session from list :  `tmux attach -t 0`
  `-t 0` -t for specific target and 0 name of the session
 	+ attach to a new session : `tmux new -s database`
  `new -s database`  new for new ,  -s for session , database as name of session
  `new -w __`  -w for new window  
 	+ rename session : `C-b $`
  rename before starting the session : `tmux rename-session -t 0 database`
+ to enter command prompt mode :  `C-b :`

NOTE : to see the more key bindings use **``C-b ?``**

 + It will show the all binding available in it

---

## Links 🔗

1. [blog](https://medium.com/hackernoon/a-gentle-introduction-to-tmux-8d784c404340)
2. [key-binds_img]()  
3. [YT-video](https://youtu.be/icEE9HHtawc)
4. tmux key binds :
 1. [default-key-binds](https://sourcedigit.com/wp-content/uploads/2014/09/Tmux-Key-Binding-Commands.png)
 2. [resize-pane-using-command](https://sourcedigit.com/wp-content/uploads/2014/09/Tmux-Resize-Pane-Commands.png)
 3. [to-control-screen](https://sourcedigit.com/wp-content/uploads/2014/09/Screen-Terminal-Multiplexer-Commands.png)
5. [key-binds](obsidian://open?vault=Obsidian&file=11%2FDaily-Note%2Ftmux-1.png)

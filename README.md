# My build of [st](https://st.suckless.org/) - simple terminal
updated to latest version 0.8.5

## Patches
* [alpha](https://st.suckless.org/patches/alpha/)
* [boxdraw](https://st.suckless.org/patches/boxdraw/)
* [copyurl-multiline](https://st.suckless.org/patches/copyurl/)
* [externalpipe](https://st.suckless.org/patches/externalpipe/)
* [font2](https://st.suckless.org/patches/font2/)
* [scrollback](https://st.suckless.org/patches/scrollback/)
* [scrollback-mouse](https://st.suckless.org/patches/scrollback/)
* [xresources-with-reload-signal](https://st.suckless.org/patches/xresources-with-reload-signal/)

## Extra features (using dmenu) copied from [Luke's build](https://github.com/lukesmithxyz/st)

* **follow urls** by pressing `alt-shift-l`
* **copy urls** in the same way with `alt-y`
* **copy the output of commands** with `alt-o`

## Xresources live-reload
```
# example

xrdb ~/.Xresources && kill -USR1 $(pidof st)
```

## Bindings
* **scroll ↑/↓ by line:** `alt-p/n`
* **scroll ↑/↓ by page:** `alt-v/ctrl-v` or `shift-Page Up/Page Down`
* **select and copy url (using coryurl patch):** `alt-l`
* **increase/decrease/reset font size:** `ctrl-=/-/0` or `ctrl-shift-Page Up/Page Down/Home`

## Installation
```
git clone https://github.com/Graphity/st.git
cd st
sudo make install clean
```

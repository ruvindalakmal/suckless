# Arch Linux Suckless Build

A minimalist, high-performance desktop environment based on Suckless tools. This repository contains my personal configurations for `dwm`, `st`, and `dmenu`, customized for Arch Linux.

## ⌨️ Keybindings

### **dwm** (Window Manager)
| Keybinding | Action |
| :--- | :--- |
| `MODKEY + Enter` | Open Terminal (st) |
| `MODKEY + d` | Open dmenu |
| `MODKEY + q` | Quit/Close Window |
| `MODKEY + Shift + Backspace` | Full Exit (Kill dwm session) |

### **st** (Terminal)
| Keybinding | Action |
| :--- | :--- |
| `Alt + c` | Copy to clipboard |
| `Alt + v` | Paste from clipboard |
| `Alt + a` | Increase Alpha (Less transparent) |
| `Alt + s` | Decrease Alpha (More transparent) |
| `Alt + Shift + k` | Increase Font Size |
| `Alt + Shift + j` | Decrease Font Size |

### **dmenu** (Launcher)
| Keybinding | Action |
| :--- | :--- |
| `MODKEY + d` | Search and launch applications |

---

## 🚀 Installation

# Install suckless Directory
git clone https://github.com/ruvindalakmal/suckless

# Install dwm
cd ~/suckless/dwm
sudo make clean install

# Install st
cd ~/suckless/st
sudo make clean install

# Install dmenu
cd ~/suckless/dmenu
sudo make clean install

## To start the environment, add the following line to your ~/.xinitrc:

exec dwm

#Then run startx from the TTY.

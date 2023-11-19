# VNC Setup for GNOME Desktop on Ubuntu

This section provides instructions for setting up VNC to access the GNOME desktop on Ubuntu.

## 5. Set Up VNC for GNOME Desktop

### 5.1 Install VNC Server

```bash
sudo apt update
sudo apt install vnc4server
```
### 5.2 Start VNC Server
```bash
vncserver :1
```

### 5.3 Set  VNC Password
```bash
vncpasswd
```
- I already set a password which is: @freedata

### 5.4 Configure VNC Session
```bash
sudo nano ~/.vnc/xstartup
```
- add to end of code
```bash
gnome-session --session=gnome-classic &
```





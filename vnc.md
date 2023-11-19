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

## 6. Connect to GNOME Classic Desktop from Windows using SSH Tunneling

```bash
ssh -L 5901:localhost:5901 username@server_ip
```
- Note: remeber to change your username and set appropriate your sever_ip

### 6.1 Connecting using  TightVNC Installer

1. **Download TightVNC Installer:**

   Visit the [TightVNC download page](https://www.tightvnc.com/download.php) and download the TightVNC Installer for Windows.

2. **Run the Installer:**

   Locate the downloaded installer file (usually a `.exe` file) and double-click to run it. Follow the on-screen instructions to install TightVNC.

3. **Connect to your VNC server and Enter password set during installation**
```bash
localhost:5901
```

### 6.2 Connecting using  RealVNCViewer Installer

1. **Download RealVNCViewer Installer:**

   Visit the [TightVNC download page](https://www.realvnc.com/en/connect/download/viewer/) and download the TightVNC Installer for Windows.

2. **Run the Installer:**

   Locate the downloaded installer file (usually a `.exe` file) and double-click to run it. Follow the on-screen instructions to install TightVNC.

3. **Connect to your VNC server and Enter password set during installation**
```bash
localhost:5901
```
   
   






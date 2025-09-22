<p align="center">
 <img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/9c6deb27-f781-408d-8757-b8f77038a015" />

</p>

---

The **Dashboard** provides a quick overview of the server’s status, resource usage, active services, and traffic information.  
It is divided into several sections with real-time updates.


----

### Activation Tutorial

To activate the web panel, read this [link](https://returnfi.github.io/Blitz-docs/menu/advance-menu/#8-web-panel).


---

## System Overview

At the top, four info boxes display core server metrics:

- **CPU Usage** → Current CPU load percentage.  
- **RAM Usage** → Memory usage vs total RAM.  
- **Online Users** → Number of currently connected users.  
- **Uptime** → How long the server has been running since the last reboot.  

---

## Network & Connections

- **Network Speed**  
  - Shows **Download** and **Upload** speeds in real time.  

- **Active Connections**  
  - Displays the number of active **TCP** and **UDP** connections.  

- **Server IPs**  
  - Shows the **IPv4** and **IPv6** addresses of the server.  
  - By default, IPs are blurred for privacy.  
  - Click the <kbd>👁</kbd> icon to toggle visibility.  

---

## Traffic Statistics

Two cards provide traffic usage details:

1. **Traffic Since Last Reboot**  
   - Uploaded traffic  
   - Downloaded traffic  
   - Combined total  

2. **User Traffic (All Time)**  
   - Total uploaded by users  
   - Total downloaded by users  
   - Combined total  

---

## Service Status

The dashboard also monitors the status of integrated services.  
Each box shows whether the service is **Active** (green) or **Inactive** (red):

- **Hysteria2 Core**  
- **Telegram Bot**  
- **IP Limit Service**  
- **Subscription Service**  

---

## How It Works

- Data is fetched automatically from two backend APIs:  
  - `server_status_api` → System metrics & traffic stats  
  - `server_services_status_api` → Service statuses  

- **Refresh Intervals**:  
  - System info updates every **2 seconds**.  
  - Service statuses update every **10 seconds**.  

- **Interactive Elements**:  
  - Toggle server IP visibility (blur/unblur).  

---

## Key Notes

- All statistics are real-time and refresh automatically.  
- If a service is down, its status box will turn **red (Inactive)**.  
- Use this page as the primary monitoring tool for server health.  


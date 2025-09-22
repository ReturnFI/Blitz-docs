## Settings Page Description

<p align="center">
 <img src="https://github.com/user-attachments/assets/0853e535-f4ce-4c24-989e-8dc5bdf4d58f" width="800" height="900">
</p>

---

# Settings Page Guide

This document provides a comprehensive guide to all the available options on the Settings page. The page is organized into several tabs, each managing a specific aspect of the service.

## Subscriptions

This tab manages the web server that provides subscription links to users.

### Service Control

This is the primary control for the subscription service.

*   **Domain:** Enter the domain name (e.g., `sub.yourdomain.com`) where the subscription service will be accessible. Do **not** include `http://` or `https://`.
*   **Port:** Specify the port on which the service will listen (e.g., `8080`).
*   **Start Service:** After filling in the domain and port, click this button to start the web server.
*   **Stop Service:** If the service is running, this button will appear to allow you to stop it.

### Configure Link

This sub-tab becomes visible only after the subscription service has been started. It allows you to customize the URL path for subscription links.

*   **Subscription Path Segment:** Enter a unique, simple string (e.g., `my-sub`) to create a custom path. This helps in making the subscription links less predictable. For example, using `my-sub` will result in links like `http://sub.yourdomain.com:8080/my-sub/...`.
*   **Save Subpath:** Click to apply the new path segment.

## Telegram Bot

This tab allows you to integrate and manage a Telegram bot for administrative tasks and notifications.

*   **API Token:** Enter the unique token for your Telegram bot, obtained from the BotFather.
*   **Admin ID:** Enter your numerical Telegram User ID to grant yourself administrative privileges for the bot.
*   **Automatic Backup Interval (Hours):** Set a schedule for how often the bot should automatically back up your configuration (e.g., `12` for every 12 hours).
*   **Start:** After entering the API Token and Admin ID, click to start the bot.
*   **Stop:** If the bot is running, this button will stop it.
*   **Save Interval:** While the bot is running, you can update the backup interval and click this button to save the change without restarting the bot.

## Hysteria Settings

This section contains core configuration options for the Hysteria service itself.

*   **Change Port:** Modify the main port that the Hysteria service uses to listen for client connections.
*   **Change SNI:** Set or change the Server Name Indication (SNI) domain. This is used to mimic traffic to a legitimate website, helping to avoid detection.
*   **OBFS:** Enable or disable obfuscation (OBFS) for your Hysteria traffic. The current status is displayed, and you can toggle it with the **Enable/Disable OBFS** buttons.
*   **Update GeoIP & GeoSite Files:** Use the buttons to download the latest GeoIP and GeoSite database files for specific countries (Iran, China, Russia). This is crucial for correctly applying routing rules.

## IP Management

This tab is for managing the IP addresses and external server nodes associated with your setup.

### Local Server IP / Domain

Define the primary IP addresses that will be embedded in user configuration links.

*   **IPv4 / Domain:** Enter the public IPv4 address or a domain name for the server.
*   **IPv6 / Domain:** Enter the public IPv6 address or a domain name for the server.

### External Nodes

If you have a multi-server setup, you can add external nodes here. These nodes will be available for inclusion in user configurations.

*   **Add New Node:**
    1.  Enter a descriptive **Node Name** (e.g., `Node-US`).
    2.  Enter the **IP Address / Domain** of the external server.
    3.  Click **Add Node**.
*   **Manage Nodes:** The table lists all configured external nodes. You can delete a node by clicking the **Delete** button in its row.

## Extra Configs

This feature allows you to add external proxy links (such as Vmess, Vless, SS, or Trojan) to all users' subscription links automatically.

*   **Add New Configuration:**
    1.  Enter a unique **Name** for the configuration (e.g., `My-Vmess-Link`).
    2.  Paste the full proxy **URI** (e.g., `vmess://...`).
    3.  Click **Add Config**.
*   **Manage Configurations:** The table lists all added configurations. You can delete any of them using the **Delete** button.

## Backup

This section provides tools for backing up and restoring your entire panel and Hysteria configuration.

*   **Restore from Backup:**
    1.  Click **Choose File** and select a previously downloaded `.zip` backup file.
    2.  Click **Upload and Restore**. A confirmation dialog will appear. The system will be restored to the state in the backup file.
*   **Create New Backup:**
    1.  Click **Download Backup** to generate and download a `.zip` file containing a full backup of your current settings.

## IP Limit

This tab controls a service that limits the number of IP addresses a single user can connect from simultaneously.

### Service Control

*   **Start:** Click to enable the IP limiting service.
*   **Stop:** Click to disable the service.

### Configuration

This sub-tab is only active when the service is running.

*   **Block Duration (seconds):** Set the amount of time in seconds that an IP address will be blocked after exceeding the limit.
*   **Max IPs per User:** Define the maximum number of simultaneous IP addresses allowed for a single user.
*   **Save Configuration:** Click to apply your changes.

## Decoy Site

Set up a decoy website to serve as a plausible front for your proxy service, making it harder to identify.

*   **Domain:** Enter the domain that will point to your decoy site.
*   **Decoy Site Path:** Provide the absolute path on the server where the decoy website's files (e.g., `index.html`) are located.
*   **Setup Decoy:** Click to configure and start the decoy site service.
*   **Stop Decoy:** If a decoy site is active, this button will appear to stop it.
*   **Status:** The current status (Active or Not Active) is displayed on this tab.

## WARP

This tab allows you to manage the Cloudflare WARP service to route your server's outgoing traffic.

*   **Install & Start WARP:** If WARP is not active, this button will install and start the service.
*   **Stop & Uninstall WARP:** If WARP is active, this button will stop and completely remove the service.

### WARP Routing Configuration

When WARP is active, you can configure its routing behavior:

*   **Route All Traffic through WARP:** Forces all of the server's outgoing traffic through the WARP network.
*   **Route Popular Sites through WARP:** Only routes traffic to popular international sites through WARP.
*   **Route Domestic Sites through WARP:** Only routes traffic to domestic sites (based on GeoIP) through WARP.
*   **Block Adult Sites (WARP Family DNS):** Enables WARP's DNS filter to block adult content.
*   **Save Configuration:** Click to apply your selected routing rules.
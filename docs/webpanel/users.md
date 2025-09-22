### User Page Description

<p align="center">
 <img src="https://github.com/user-attachments/assets/cca881cb-57bd-49b5-808f-6c099c937ede" width="900" height="700">
</p>

This page is designed for **user management**. You can **view, search, filter, add, edit, and delete** users. It also provides the ability to **display QR Codes** and **extract links**.

---

## Main Features

### 1. User List
The user table contains the following information:

| Column | Description |
|--------|-------------|
| **Username** | Unique username of the user |
| **Status** | User status: `Online`, `Offline`, `Hold`, or `Conflict` |
| **Traffic Usage** | Amount of traffic used and total limit |
| **Expiry Date & Days** | Expiration date and remaining days |
| **Day Usage** | Number of days the user has used the service |
| **Enable/Disable** | Whether the account is active or disabled |
| **Configs (QR Codes)** | View and copy connection configs (IPv4, IPv6, Normal SUB) |
| **Actions** | Management buttons including **Edit**, **Reset**, and **Delete** |

> **Note:**  
> On mobile view, user details are shown in an **accordion (collapsible)** format to keep the table compact.

---

### 2. User Filters

At the top of the table, buttons are provided to filter users:

- `All`: Show all
- `Hold`: Show users with **Hold** status
- `Online`: Show online users
- `Enable`: Show active users
- `Disable`: Show disabled users

On mobile, these filters are available in a **Dropdown**.

---

### 3. Search

At the top-right of the table, there is a **Search** field.  
Simply type part of a username and the list will be automatically filtered.

---

### 4. Add User

Click the <kbd>+</kbd> button to open a **Modal**.

#### Single User (Add User)

- **Username** (required, only letters, numbers, and `_`)
- **Traffic Limit (GB)**
- **Expiration Days**
- **Unlimited IP** (only if IPLimit service is enabled)

#### Bulk Add
This mode allows you to add multiple users at once. Options include:

| Option | Description |
|--------|-------------|
| **Username Prefix** | Prefix for usernames (e.g., `user`) |
| **Number of Users** | Number of users to be created (e.g., 10) |
| **Start Number** | Starting number (e.g., if 5, the users will be `user5`, `user6`, ...) |
| **Traffic Limit (GB)** | Traffic limit for all bulk users |
| **Expiration Days** | Expiration days for all bulk users |
| **Unlimited IP** | If enabled, users will not have IP restrictions |

---

### 5. Edit User

The ✏️ **Edit** button is available next to each user. You can:

- Change the **Username**
- Change the **Traffic Limit**
- Change the **Expiration Days**
- **Block/Unblock** the user
- Enable/Disable the **Unlimited IP** option

---

### 6. Reset & Delete

- **Reset (↩):** Reset the user  
- **Delete (🗑):** Completely remove the user  

You can also select multiple users and delete them in bulk.

---

### 7. QR Code

By clicking on the **QR Code** icon, you can view the user’s configs:

- IPv4
- IPv6
- Normal SUB

Each QR is clickable, and clicking will copy the link to your clipboard.

---

### 8. Extract Links

You can select multiple users and click the **🔗 Show Links** button.  
A **Modal** will open, allowing you to choose:

- IPv4
- IPv6
- Normal SUB
- Nodes

Then you can:

- **Extract** the links  
- **Copy** all links at once  

---

## Important Notes

- Validation is applied on **Username** (only `a-z`, `A-Z`, `0-9`, `_` are allowed).  
- If the **IPLimit** service is enabled, options related to `Unlimited IP` will be visible.

---

## Shortcuts
- <kbd>+</kbd> → Add User
- <kbd>🔍</kbd> → Search
- <kbd>🗑</kbd> → Delete user(s)
- <kbd>🔗</kbd> → Show links
- <kbd>📶</kbd> → Filter Online status

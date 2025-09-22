### Users Page Description

<p align="center">
 <img src="https://github.com/user-attachments/assets/cca881cb-57bd-49b5-808f-6c099c937ede" width="900" height="700">
</p>

This page is designed for managing users. You can **view, search, filter, add, edit, and delete** users. It also provides options to **display QR Codes** and **extract links**.

---

## Main Features

### 1. User List
- The user table includes:
  - **Username**
  - **Status** (Online, Offline, Hold, Conflict)
  - **Traffic Usage**
  - **Expiry Date & Days**
  - **Day Usage**
  - **Enable/Disable**
  - **Configs (QR Codes)**
  - **Actions (Edit, Reset, Delete)**

> On mobile, user details are shown in an **accordion view** for better readability.

---

### 2. User Filters
At the top of the table, there are buttons to filter users:
- `All` : Show all users
- `Hold` : Show users with **Hold** status
- `Online` : Show online users
- `Enable` : Show enabled users
- `Disable` : Show disabled users

On mobile, these filters are grouped inside a **Dropdown** menu.

---

### 3. Search
- A **Search** field is available at the top-right of the table.
- Simply type part of a username to automatically filter the list.

---

### 4. Add User
Click the <kbd>+</kbd> button to open a **modal window**.

#### Single User (Add User)
- **Username** (required, only letters, numbers, and `_`)
- **Traffic Limit (GB)**
- **Expiration Days**
- **Unlimited IP** (if the IPLimit service is enabled)

#### Bulk Add
- **Username Prefix**
- **Number of Users**
- **Start Number**
- **Traffic Limit**
- **Expiration Days**
- Option to enable **Unlimited IP**

---

### 5. Edit User
- The ✏️ Edit button is available next to each user.
- You can:
  - Change the **Username**
  - Change the **Traffic Limit**
  - Change the **Expiration Days**
  - **Block/Unblock** the user
  - Enable/disable the **Unlimited IP** option

---

### 6. Reset & Delete
- **Reset (↩):** Reset a user
- **Delete (🗑):** Permanently delete a user
- Multiple users can be selected and deleted in bulk.

---

### 7. QR Code
- By clicking the **QR Code** icon, you can view the user’s configurations:
  - IPv4
  - IPv6
  - Normal SUB
- Each QR code is clickable, and the corresponding link will be copied to the clipboard.

---

### 8. Extract Links
- Select multiple users and click the **🔗 Show Links** button.
- A **modal window** will appear allowing you to choose:
  - IPv4
  - IPv6
  - Normal SUB
  - Nodes
- You can then:
  - **Extract** the links
  - **Copy** all links at once

---

## Important Notes
- All requests are connected to backend APIs (Flask).
- **Username validation** is applied (only `a-z`, `A-Z`, `0-9`, `_` are allowed).
- If the **IPLimit** service is active, options related to `Unlimited IP` will be visible.

---

## Shortcuts
- <kbd>+</kbd> → Add User  
- <kbd>🔍</kbd> → Search  
- <kbd>🗑</kbd> → Delete User(s)  
- <kbd>🔗</kbd> → Show Links  
- <kbd>📶</kbd> → Filter Online Users  


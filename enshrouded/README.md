# Enshrouded

### Game Description

Enshrouded is a game of survival, crafting, and Action RPG combat, set within a sprawling voxel-based continent. As you journey across the mountains and deserts of an open world, you are free to choose your path and shape your destiny.

Ignite the Ancient power of the Flame, and piece together the fragments of a story that unfolds below the surface.

### Usefull links

- Homepage: https://enshrouded.com/
- Steam: https://store.steampowered.com/app/1203620/Enshrouded/
- Wiki: https://enshrouded.wiki.gg/wiki/Enshrouded_Wiki
- Discord: https://discord.gg/enshrouded

### Author & Contributers
| Name        | Github Profile  | Buy me a Coffee |
| ------------- |-------------|-------------|
|   Red-Banana-Official  | https://github.com/Red-Banana-Official | / |
|   Vapok   | https://github.com/Vapok | https://www.buymeacoffee.com/vapok |
|   QuintenQVD0   | https://github.com/QuintenQVD0 | / |
|   gOOvER   | https://github.com/gOOvER | https://ko-fi.com/B0B351D0Q  |

### Server Ports

Enshrouded requires up to 2 ports. Queryport must be GAMEPORT +1 

| Port    | default       |
|---------|---------------|
| Game    |     15636     |
| Query   |     15637     |

## Configuration

### **Where is the Server Configuration Stored?**
The Enshrouded dedicated server configuration is stored in `enshrouded_server.json`, which is automatically managed by this egg.

Instead of manually editing this file, **you can set most key values directly in the Pterodactyl Panel** using environment variables.

---

### **How to Configure the Server**
**Most settings can be modified via Pterodactyl's environment variables.**  
Go to your **Pterodactyl Panel → Server Settings**, where you can edit:
- **Server Name (`SRV_NAME`)** – The name players will see in the server list.
- **User Group Passwords**:
  - **Default Group (`SRV_PW`)** – General access for most players.
  - **Admin Group (`SRV_PW2`)** – Grants admin privileges.
  - **Friends Group (`SRV_PW3`)** – Grants reduced admin privileges.
- **Max Players (`MAX_PLAYERS`)** – Number of player slots (1-16).
- **Steam Query Port (`QUERY_PORT`)** – The query port for server communication.

Other settings, such as **game settings, IP binding, and log locations**, are still managed in `enshrouded_server.json`

---

### **Default Configuration File (`enshrouded_server.json`)**
On first startup, the server will generate the following structure:

```json
{
    "name": "My Server",
    "saveDirectory": "./savegame",
    "logDirectory": "./logs",
    "ip": "0.0.0.0",
    "gamePort": 15636,
    "queryPort": 15637,
    "slotCount": 16,
    "userGroups": [
        {
            "name": "Default",
            "password": "ChangeMe",
            "canAccessInventories": true,
            "canEditBase": true,
            "canExtendBase": true,
            "canKickBan": false,
            "reservedSlots": 0
        },
        {
            "name": "Admins",
            "password": "ChangeMe",
            "canAccessInventories": true,
            "canEditBase": true,
            "canExtendBase": true,
            "canKickBan": true,
            "reservedSlots": 1
        },
        {
            "name": "Friends",
            "password": "ChangeMe",
            "canAccessInventories": true,
            "canEditBase": true,
            "canExtendBase": true,
            "canKickBan": false,
            "reservedSlots": 3
        }
    ],
    "voiceChatMode": "Proximity"
}
```

### Installation/System Requirements

|           | Recommended  | Extra info  |
|-----------|--------------|-------------|
| Processor | Recent x86/64 (AMD/Intel) processor. | You need min 4 Cores for the Server. |
| RAM       |  4-6 GB     |
| Storage   |  30 GB (or more, depending on save size or frequency) |

### Server not showing in Serverlist?

The fact that the server is not displayed in the server list is a known problem.

As a workaround, you can add the server as a favourite via IP:port in the Steam server browser.
The server should then be at the top of the ingame server list

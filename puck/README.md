# Puck
### Game Description

Hop on your skates and jump into a physics based hockey game. No rules, no timeouts, just get the puck in the goal. May the best team win!

### Usefull links

- Steam: https://steamcommunity.com/app/2994020

### Author & Contributers
| Name        | Github Profile  | Buy me a Coffee |
| ------------- |-------------|-------------|
|   Red-Banana-Official  | https://github.com/Red-Banana-Official | / |
|   Rai68   | https://github.com/rai68 | / |

### Server Ports

By default Puck requires 2 ports.

| Port    | default       |
|---------|---------------|
|Game    |     7777     |
|Query   |     7778     |


## Configuration

### **Where is the Server Configuration Stored?**
The Puck dedicated server configuration is stored in `server_configuration.json`, which is automatically managed by this egg.

Instead of manually editing this file, **you can set most key values directly in the Pterodactyl Panel** using environment variables.

---

### **Default Configuration File (`server_configuration.json`)**
On first startup, the server will generate the following structure:

```json
{
    "adminSteamIds": [],
    "isPublic": true,
    "kickTimeout": 300,
    "maxPlayers": 10,
    "name": "Pterodactyl Puck Server",
    "password": "",
    "phaseDurationMap": {
        "BlueScore": 5,
        "FaceOff": 3,
        "GameOver": 15,
        "PeriodOver": 15,
        "Playing": 300,
        "RedScore": 5,
        "Replay": 10,
        "Warmup": 600
    },
    "pingPort": 7778,
    "port": 7777,
    "printMetrics": true,
    "reloadBannedSteamIds": false,
    "targetFrameRate": 120,
    "tickRate": 100,
    "usePuckBannedSteamIds": true,
    "voip": false
}
```

### Installation/System Requirements

|           | Recommended  | Extra info  |
|-----------|--------------|-------------|
| Processor | Recent x86/64 (AMD/Intel) processor. | You need min 1 Core for the Server. |
| RAM       |  1 GB     |
| Storage   |  1 GB (or more, depending on save size or frequency) |

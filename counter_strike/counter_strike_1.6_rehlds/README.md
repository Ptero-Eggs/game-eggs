# Counter-Strike 1.6 ReHLDS

## Description
Counter-Strike 1.6 ReHLDS (Reverse Engineered Half-Life Dedicated Server) is an optimized and updated version of the original HLDS, designed for stability, performance, and security. It provides a modern platform for hosting Counter-Strike 1.6 servers with improved support for custom plugins and modules.

This repository offers everything you need to set up a Counter-Strike 1.6 server using ReHLDS, MetaMod-R, AMX Mod X, and other popular tools.



## Installation Notes

This repository is designed for use with Pterodactyl Panel, automating the installation process and ensuring an up-to-date setup. Follow the egg's setup instructions to deploy a fully functional server.



## System Requirements

| Component    | Minimum             | Recommended        |
|--------------|---------------------|--------------------|
| Processor    | -                   | -                  |
| RAM          | 1 GB                | 2 GB               |
| Storage      | 2 GB                | 5 GB               |



## Server Ports

The following ports are required to run a Counter-Strike 1.6 server:

| Port    | Default |
|---------|---------|
| Game    | 27015   |
| HLTV    | 27020   |

Ensure these ports are open and properly forwarded if running the server behind a firewall or router.





## Modules

- **ReHLDS**: Improved performance, crash protection, and extended features.
- **MetaMod-R**: Plugin loader for custom server modifications.
- **AMX Mod X**: Advanced scripting platform for server plugins.
- **ReAPI**: Enhances plugin capabilities with new native functions.
- **ReGameDLL**: Updated game library for improved functionality.



## Notes

- The server installation includes default configuration files such as `server.cfg`, `listip.cfg`, and `banned.cfg`.
- The `reunion.cfg` file is used for managing authentication settings.

For further configuration or plugin information, refer to the official [AMX Mod X documentation](https://amxmodx.org/) or the [ReHLDS GitHub repository](https://github.com/dreamstalker/rehlds).

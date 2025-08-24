# Nightingale

Nightingale is an open world survival crafting game, where you’ll adventure across the mysterious and dangerous Fae Realms. As a daring Realmwalker, you’ll defeat monstrous enemies, survive hostile environments, and build elaborate estates in a visually stunning Gaslamp Fantasy world

 ### Author & Contributers
| Name        | Github Profile  |
| ------------- |-------------|
|   brainshead   | https://github.com/brainshead |

## Server Ports

Nightingale requires up to 1 ports

| Port    | default       |
|---------|---------------|
| Game    | 7777          |

This can be changed to any port.

## Install Notes

| Requirements        | Memory| Storage | 
|---------------------|-------|---------|
| Minimal             | 4GB   | 15 GB   |
| Recommended         | 6-8+ GB| 40GB+  |


## Settings

Most setting can be done by Panel Variable Settings.

Location of server Files : NWX/Config/ServerSettings.ini

## Persistence (Saved Data)

Realm data is be stored in: NWX/Saved/Offline/DedicatedServer/Deploy

Character data is stored in: NWX/Saved/Offline/<PlatformID>/Profiles where

PlatformID is the Steam or Epic ID of each connecting user.

Backups

Copying the following directories to a backup location is sufficient to capture the state of a Nightingale dedicated server:

● NWX/Saved/Offline

● NWX/Saved/Config

● NWX/Config

The first time the dedicated server is launched on a particular weekday, it will copy the Offline

directory into the OfflineBackup directory.

Resetting Server Persistence

To reset the server to an empty state, remove the following directories:

● NWX/Saved/Offline

● NWX/Saved/Config




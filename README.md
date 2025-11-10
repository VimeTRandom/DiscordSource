# DiscordSource
A tf2 discord relay plugin that relays between server, and discord server


⚙️ DiscordSource Configuration String Values
This document outlines all available string variables you can use within your DiscordSource configuration files (e.g., in .cfg files) to customize message outputs.

These variables are designed to be used in conjunction with other text, numbers, or percentages to build a complete text output.

### 📝 Configuration Example
EXAMPLE


| Category | Example Value | Description |
| :--- | :--- | :--- |
| **Server Status** | `SERVER_COUNT/SERVER_MAXCLIENT` | Shows current players vs. max slots. |
| **Auth Info** | `AUTH_NAME` | The player's Steam Name. |
| **Discord Info** | `USER_NAME` | The Discord user who sent the message. |


### 🛡️ Auth Types
These variables pull information about the client (player) related to the event (e.g., joining, leaving, sending a message).

| Example Value | Description | Example Output |
| :--- | :--- | :--- |
| `AUTH_NAME` | Uses Client’s Steam Name. | `Player_Name123` |
| `AUTH_ID` | The client’s Steam ID (e.g., SteamID3 or SteamID64). | `[U:1:9653243234]` |
| `AUTH_MESSAGE` | The client’s Message content. | `Hey, what map is next?` |
| `AUTH_CONNECT` | Shows the client’s connection status (Join/Leave). | `joined the game` or `left the game` |
| `AUTH_ONLINE_STATUS` | Shows the client’s current online/offline status. | `Online` or `Offline` |


### 🚨 CallAdmin Specific (Only for calladmin.cfg)
These variables provide the rule breaker infomation

| Example Value | Description | Example Output |
| :--- | :--- | :--- |
| `AUTH_BREAKER_NAME` | The name of the reported rule breaker. | `Vime` |
| `AUTH_BREAKER_ID` | The ID of the reported rule breaker. | `[U:1:878320834]` |
| `AUTH_BREAKER_STEAM` | URL for the rule breaker's Steam Profile Page. | `https://steamcommunity.com/profiles/76561198838586562` |
| `RULE_REASON` | The reported reason/rule violation. | `Scam` |


### 🔗 Auth URL Types (Profile Links)
These variables provide URLs to the client's various profiles and pages.

| Example Value | Description | Example Output |
| :--- | :--- | :--- |
| `AUTH_AVATAR` | URL to the client's Steam Avatar. | `https://avatars.steamstatic.com/d33c7f15aee3490b26fd84249776c59156747f9d_full.jpg` |
| `AUTH_STEAM` | URL to the client’s Steam Profile Page. | `https://steamcommunity.com/profiles/76561198838586562` |
| `AUTH_BP` | URL to the client’s Backpack.tf Page. | `https://backpack.tf/u/76561198838586562` |
| `AUTH_TRADE` | URL to the client’s Trade URL (requires client cookie sqlite data). | `https://steamcommunity.com/tradeoffer/new/?partner=8782203424&token=6eE264e-A` |


### 💬 Discord Types (Discord User/Channel Information)
These variables pull information directly from the Discord side of the interaction.

| Example Value | Description | Example Output |
| :--- | :--- | :--- |
| `USER_NAME` | The Discord User’s Name. | `Tommy` |
| `USER_MESSAGE` | The Discord User’s Message content. | `I love tf2` |
| `CHANNEL_NAME` | The channel name where the message was sent. | `General` |


### 🎮 Server Source Info (Server Status)
These variables provide real-time information about the Source Game Server.

| Example Value | Description | Example Output |
| :--- | :--- | :--- |
| `SERVER_NAME` | The Source Server Name. | `My Awesome Source Server` |
| `SERVER_IP` | The Source Server IP and port. | `145.63.37.10:27312` |
| `SERVER_MAP` | The Source Server Current Map. | `ctf_2fort` |
| `SERVER_COUNT` | The Source Server Current Player Count. | `15` |
| `SERVER_MAXCLIENT` | The Maximum Player Slots of the server. | `32` |
| `SERVER_PERCENT` | The Percentage of players relative to Max Slots. | `46.87%` |
| `SERVER_REGION` | The Region of The Source Server. | `Europe` |

Adding more in the future

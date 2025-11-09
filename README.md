# DiscordSource
A tf2 discord relay plugin that relays between server, and discord server


DiscordSource Configuration String Values
Note: These are string variables. You can use them in conjunction with other values (e.g., numbers or percentage) to build a complete text output, such as a message displaying the player count and percentage.

EXAMPLES:

"SERVER_COUNT/SERVER_MAXCLIENT – SERVER_PERCENT" = "3/32 – 8.82%"

"IP: (SERVER_IP) | Player Count: (SERVER_COUNT/SERVER_MAXCLIENT) || SERVER_PERCENT" = "IP: (145.63.37.10:27312) | Player Count: (3/32) || 8.82%"

🛡️ Auth Types
AUTH_NAME - Uses the Client’s Steam Name.

AUTH_ID - Uses the Client’s ID (e.g., Steam ID).

AUTH_MESSAGE - Uses the Client’s Message (the text input).

AUTH_CONNECT - Shows the Client’s connection status (e.g., "left the game" or "joined the game").

AUTH_ONLINE_STATUS - Shows the Client’s online/offline status (e.g., "Online" or "Offline").

CallAdmin Specific (Only in calladmin.cfg)
AUTH_BREAKER_NAME - Shows the name of the rule breaker being reported.

AUTH_BREAKER_ID - Shows the ID of the rule breaker being reported.

AUTH_BREAKER_STEAM - Shows the rule breaker's Steam Profile Page URL.

RULE_REASON - Shows the reported reason/rule violation.

🔗 Auth URL Types
AUTH_AVATAR - Shows the Client's Steam Avatar URL.

AUTH_STEAM - Shows the Client’s Steam Profile Page URL.

AUTH_BP - Shows the Client’s Backpack.tf Page URL.

AUTH_TRADE - Shows the Client’s Trade URL (requires client cookie sqlite data).

AUTH_CUSTOM - Uses a Custom Link constructed with the Client’s steamID64.

💬 Discord Types
USER_NAME - Uses the Discord User’s Name.

USER_MESSAGE - Uses the Discord User’s Message content.

CHANNEL_NAME - Uses the channel name where the message was sent.

🎮 Server Source Info
SERVER_NAME - Shows the Source Server Name.

SERVER_IP - Shows the Source Server IP and port.

SERVER_MAP - Shows the Source Server Current Map.

SERVER_COUNT - Shows the Source Server Current Player Count.

SERVER_MAXCLIENT - Shows the Maximum Player Slots of the server.

SERVER_PERCENT - Shows the Percentage of players in the server relative to Max Player Slots (e.g., "9.37%").

SERVER_REGION - Shows the Region of The Source Server.

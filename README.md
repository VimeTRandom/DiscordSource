# DiscordSource
A tf2 discord relay plugin that relays between server, and discord server


These are All the available Sting Values you can USE for DiscordSource cfg’s files

Note: These are string variables. You can use them in conjunction with other values (e.g., numbers or percentage) to build a complete text output, such as a message displaying the player count and percentage.

EXAMPLES:
“SERVER_COUNT/SERVER_MAXCLIENT – SERVER_PERCENT” = “3/32 – 8.82%”
And I can add more

“IP: (SERVER_IP) | Player Count: (SERVER_COUNT/SERVER_MAXCLIENT)  || SERVER_PERCENT” 
= IP: (145.63.37.10:27312) | Player Count: (3/23) || 8.82%

Auth Types

AUTH_NAME - Uses Client’s Steam Name
AUTH_ID - Uses Client’s ID
AUTH_MESSAGE - Uses Client’s Message
AUTH_CONNECT - Shows Client’s connection = “lefted the game” or “joined the game”
AUTH_ONLINE_STATUS - Shows Client’s Online/Offline status = “Online” or “Offline”


AUTH_BREAKER_NAME - Shows the name of a rule breaker in calladmin (only in calladmin.cfg)
AUTH_BREAKER_ID - Shows the ID of rule breaker (only in calladmin.cfg)
AUTH_BREAKER_STEAM - Shows rule breaker Steam Page (only in calladmin.cfg)
RULE_REASON - Shows the rule that was reported  (only in calladmin.cfg)
-

Auth Url Types

AUTH_AVATAR - Client's Steam Avatar
AUTH_STEAM - client’s Steam Page
AUTH_BP - client’s Backpack.tf Page
AUTH_TRADE - client’s Trade URL (Uses client cookie sqllite)
AUTH_CUSTOM - uses a Custom Link with Client’s steamid64: 


Discord Types:

USER_NAME - User’s Discord Name
USER_MESSAGE - User’s Discord Message
CHANNEL_NAME - channel name where is message was sent

Server Source Info

SERVER_NAME - Source Server Name
SERVER_IP - Source Server IP
SERVER_MAP - Source Server Current Map
SERVER_COUNT - Source Server Player Count
SERVER_MAXCLIENT - Source Server Gets the MAX Player Slots of the server
SERVER_PERCENT -  Percentage of players in the server relative to PLayer Slots EX(9%)
SERVER_REGION - Region of The Source Server

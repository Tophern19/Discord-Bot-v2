# Discord-Bot-v2
It is a discord bot that manages servers there is a list that tells you all the commands in the file all you need to do is 
LISTEN THE RICKROLL FUNCTION DOES NOT WORK IT JUST MUTES YOU SERVER SO AVOID USING IT IM WORKING TO FIX IT SORRY AND HERE ARE THE COMMANDS (PS IF DOWNLOADING IT DOESNT WORK [MAKE SURE YOU TYPE NODE BOT.JS REMOVE THE 1 AND .TXT TO CHANGE TO A .JS FILE AFTER UPLOADING YOUR DISCORD ID SO IT IDENTIFYS YOU AS A OWNER AND THE BOT TOKEN PLEASE GIVE ME CREDIT THANK YOU.] THEN TYPE THESE THING How to Install the Bot 1. Install Node.js

You need Node.js  18 or higher  
Download: https://nodejs.org Check version: node -v
2. Install Dependencies
Open a terminal inside the bot folder and run:
npm install
This installs discord.js  and everything else the bot needs.
3. Add Your Bot Token
Open bot.js and find:
const BOT_TOKEN = "YOUR_TOKEN_HERE";
Replace it with your actual bot token from the Discord Developer Portal.
⚠️ Never share your token.
4. Make Sure the Logs Folder Exists
Your bot needs a folder named:
logs
Inside it, create these files if they don’t exist:
Execution-logs.txt
Promotion-logs.txt
Demotion-logs.txt
Lockdown-logs.txt
punishdata.json
rickroll_leaderboard.json
Put {} inside the .json files.
5. Add the Rickroll Video
Place your video file in the same folder as bot.js.
Important:  
Discord bots cannot upload files larger than 8 MB.
Your file should be named:
Rick_Astley_Never_Gonna_Give_You_Up.mp4
(or change the filename in your code)
6. Invite the Bot to Your Server
In the Discord Developer Portal:
Go to OAuth2 → URL Generator
Select:
bot
applications.commands
Under Bot Permissions, enable:
Administrator
(or at least Manage Channels, Manage Roles, Timeout Members)
Copy the link → paste in browser → invite bot.
7. Run the Bot
In the bot folder:
Type cmd then
node bot.js
⚔️ Bot Commands & What They Do
Here are all the commands your bot supports, explained clearly.
🔨 Moderation Commands
!execute <user>
Starts a vote to mute a user for 1 week.
👍 = Yes

👎 = No
Vote lasts 30 seconds
If Yes wins → user is muted
If someone tries to execute the owner → they get muted instead, longer each time
!promote <user>
Gives the user the Moderator role.
Only the owner or moderators can use this.
!demote <user>
Removes the Moderator role from a user.
!forgive <user>
Unmutes or unbans a user instantly.
🔒 Lockdown System
!lockdown #channel [time]
Locks one or more channels so nobody can talk.
Examples:
!lockdown #general
!lockdown #general 30m
!lockdown #general 2h
Default time: 8 hours
!unlock
Ends the lockdown early.
Owner‑only command.
🎵 Rickroll Punishment System
!rickroll
Starts the full Rickroll event:
Sends Rick Astley
Locks the channel
After the video, users must pass a 10‑question quiz
Score 7/10 to unlock
Fail → try again
Pass/fail stats saved to leaderboard
Only owner/mods can run this.
!unrickroll
Instantly ends the Rickroll event and unlocks the channel.
!rickroll-leaderboard
Shows who passed/failed the Rickroll quiz the most.
📝 Important Notes
Mods and the owner do not get locked during Rickrolls

The quiz only appears when a muted user tries to talk

The bot logs everything in the /logs folder

The Rickroll video must be under 8 MB

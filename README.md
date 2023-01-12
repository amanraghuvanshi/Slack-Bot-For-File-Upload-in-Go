# Slack-Bot-For-File-Upload-in-Go
BOT FOR SLACK FOR FILE UPLOAD
SLACK BOT USING GOLANG 
INITIALIZE go.mod file and other useful resources
Along with this you need to have a slack account and a channel for broadcasting the bot.

After creating these go to #api.slack.com/apps
1. Go to Socket Mode and Enable it
2. Enable Event Subscription
3. Now to OAuth and Permissions, go to scopes and give the nessecary permission like channels:read, chat:write, files:read etc
4. After this scroll up and there will be OAuth Tokens for Your Workspace, and initialize it to get your token and store it, also mentioning store your channel ID, you can get in from Channel details or URL of channel
Along with this
For this project, we need some additional modules from the github
> go get github.com/slack-go/slack

After initialzing our go mod, we are good to start the project

Modules Needed:
	# fmt
	# os
	# github/slack-go/slack
		This module already has the network call predefined and hence we can directly call the API using the methods

1. We will be setting up our enviroment since we are not in production enviroment and hence I suggest the same
2. We will be setting enviroment for both the TOKEN and the CHANNEL through which we will be broadcasting
3. There will be a variable defined to store the store the API TOKEN for the BOT
4. An array for storing the CHANNEL_ID
5. An array to store the FILES 
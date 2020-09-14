# Teams Proactive Message

I built this project because I couldn't find a simple example of how to [send proactive messages](https://docs.microsoft.com/en-us/microsoftteams/platform/bots/how-to/conversations/send-proactive-messages) to users/channels in Microsoft Teams. Every example either started with a user sending a message to my bot (and thus had pre-existing Teams context), or had a ton of other functionality wrapped around the proactive message. This project is meant to be the most basic implementation of proactive messages. This project is not production-ready nor a representation of how you should do this for reals.

## Prerequisites

### Register your bot

TODO: Register

TODO: Enable Teams channel

### Pick a Teams channel and get its ID
TODO: use the Teams web client to figure out the channel id

TODO: install your bot in the channel (link to requirements)

[Enable proactive bot installation and proactive messaging in Teams with Microsoft Graph (Public Preview)](https://docs.microsoft.com/en-us/microsoftteams/platform/graph-api/proactive-bots-and-messages/graph-proactive-bots-and-messages?tabs=csharp)

## How to test

### Configure the API project
1. Create appsettings.Development.json (if there isn't one already) under appsettings.json
2. Copy settings from appsettings.json to appsettings.Development.json
```
	"MicrosoftAppId": "YOUR BOT ID",
	"MicrosoftAppPassword": "YOUR BOT SECRET",
	"ChannelId": "TEAMS CHANNEL ID (SHOULD START WITH SOMETHING LIKE 19:blahblahblah)",
	"ConversationsUrl": "https://smba.trafficmanager.net/amer/v3/conversations"
```
3. Populate MicrosoftAppId, MicrosoftAppPassword, and ChannelId using the values you copied from Prerequisites

### Call your API with PostMan

TODO: include collection

TODO: post a new message

TODO: update a posted message
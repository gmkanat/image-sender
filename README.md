## Telegram bot for getting random photos from Unsplash

This is a Telegram bot that uses the Unsplash API to get random photos and sends them to users who send a specific command or message. The bot is written in Go and uses the `github.com/go-telegram-bot-api/telegram-bot-api/v5` package for interacting with the Telegram Bot API and the `github.com/joho/godotenv` package for loading environment variables from a `.env` file.
### Prerequisites

To run this bot, you will need to create a Telegram bot and 
obtain a bot token, as well as an access key for the Unsplash API. 
You can create a Telegram bot by following the instructions 
[here](https://core.telegram.org/bots#creating-a-new-bot). 
To obtain an access key for the Unsplash API, 
you will need to create an account on the Unsplash website
and follow the instructions [here](https://unsplash.com/developers).

### Installation
1. Clone the repository
2. Change into the project directory
3. Create a `.env` file with the following contents:

```makefile

BOT_TOKEN=<your Telegram bot token>
UNSPLASH_ACCESS_KEY=<your Unsplash access key>
```


1. Install dependencies: `go mod tidy`
2. Build the executable: `go build`
3. Run the executable: `./telegram-unsplash-bot`
### Usage

To use the bot, add it to a Telegram group or start a chat with it. 
You can then send the command `/image` or the message `image` 
to get a random photo from Unsplash.
### License

This project is licensed under the terms of the MIT license.

# GoIP2Telegram

**GoIP SMS Forwarder to Telegram**

This PHP script is designed to forward SMS messages received from a GoIP SMS server (http://en.dbltek.com/Software-Download.html) to a Telegram group. It allows you to receive SMS notifications in your Telegram group chat, making it useful for various notification and alerting purposes.

**How it works:**
1. It listens for incoming POST requests containing SMS details from a GoIP SMS server.
2. Extracts the "number" and "content" fields from the incoming POST data.
3. Formats the extracted data into a message.
4. Sends the message to a designated Telegram group using the Telegram Bot API.

**Usage:**
1. Create a Telegram bot and obtain its token.
2. Determine the chat ID of your Telegram group.
3. Configure the script with your bot token and chat ID.
4. Set up your GoIP SMS server to send incoming SMS details to this script via POST requests (System Manage -> GoIP Manage -> Modify -> chek 'Forward SMS to HTTP' and plase url http://your-host/message.php).

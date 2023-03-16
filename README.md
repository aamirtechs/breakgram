# Employee Break Management Bot
The Employee Break Management Bot is a Telegram bot that helps organizations manage employee breaks. It allows employees to mark when they start and end their breaks, and ensures that no more than two employees are on break at the same time. If more than two employees want to take a break, the bot will put them in a queue and notify them when it is their turn to take a break.

# Getting Started
To use the Employee Break Management Bot, you will need to set up a Telegram bot and a Google Sheets API project. You will also need to share your Google Sheet with the service account email address.

# Setting up the Telegram Bot
Create a new bot in Telegram by talking to the BotFather and obtaining a bot token.
Invite your bot to your chat or channel.
Copy the bot token to the config.py file.


# Setting up the Google Sheets API
Create a new project in the Google Cloud Console.
Enable the Google Sheets API for your project.
Create a service account key for your project and download the key file.
Share your Google Sheet with the service account email address.
Copy the service account key file to the same directory as the main.py file.
Rename the service account key file to creds.json.
Installing Dependencies
You will need to install the following Python packages to run the Employee Break Management Bot:

Copy code
pip install python-telegram-bot google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client
Running the Bot
To run the Employee Break Management Bot, simply run the main.py file using Python:

css
Copy code
python main.py
The bot will start listening for commands in your chat or channel.

# Commands
The Employee Break Management Bot supports the following commands:

/start - Displays a welcome message and the available commands.
/break - Marks the start of a break for the user. If two or fewer employees are currently on break, the user will be added to the list of employees on break. If more than two employees are on break, the user will be added to the break queue and notified when it is their turn to take a break.
/end - Marks the end of a break for the user. The user will be removed from the list of employees on break, and the next employee in the break queue (if any) will be notified that it is their turn to take a break.
/queue - Displays the current break queue, if any.
Contributing
If you have any issues or feature requests, please open an issue on the GitHub repository. Pull requests are also welcome!

# License
This project is licensed under the MIT License. See the LICENSE file for details.

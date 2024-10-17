# Script Bot HTown to Discord Webhook Integration

This guide explains how to install the `requests` and `discord_webhook` libraries, set up a Discord webhook, and configure it as an environment variable for use in your Python scripts.

## Requirements

- Python (version 3.x recommended)
- Internet access for downloading packages
- Requests
- Discord_webhook

## Installation

1. **Open your terminal (Mac/Linux) or command prompt (Windows).**

2. **Install the required libraries:**

   - To install the `requests` library, run:
     ```bash
     pip install requests
     ```

   - To install the `discord_webhook` library, run:
     ```bash
     pip install discord-webhook
     ```

3. **Creating a Discord Webhook**
    Go to your Discord server settings and navigate to the channel where you want to receive messages.
    Click on Integrations and then on Webhooks.
    Click New Webhook, give it a name, and copy the Webhook URL

4. **Update weebhooks variables**
    Open script.py and put url to weebok in 13 
    DISCORD_WEBHOOK_HTOWN 

    Open common_utils.py and put url to weebok in 77 
    DISCORD_WEBHOOK_HTOWN 

    Open script.py and change line 44
    PASSARO_ONLY = False 
    if for true he goes alone to the clawser, if for false he does not go alone.
    If false you can use it on other mobs

5. **Run Script**
    You need open script.py in uostealth, run he.
    Magical
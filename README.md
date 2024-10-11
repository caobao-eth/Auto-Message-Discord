# Discord Auto Message Bot

This is a simple bot for sending and deleting messages in a Discord channel at regular intervals. It sends messages from a `.txt` file and manages their deletion after a specified period. The process repeats in a loop once all messages have been sent.

## Features
- **Automatic message sending**: Sends messages sequentially from a `.txt` file.
- **Message deletion**: Deletes the message after a delay.
- **Configurable timing**: Sends and deletes messages with configurable delays.
- **Endless loop**: Repeats the process once all messages are sent.

## How it Works
The bot reads messages from a `messages.txt` file. Each line in this file is treated as a separate message. The bot works in the following sequence:
1. **Send a message**: The bot posts a message to a specified Discord channel.
2. **Wait 60 seconds**: After sending the message, the bot waits for 60 seconds.
3. **Delete the message**: The bot deletes the previously sent message from the channel.
4. **Wait 30 seconds**: After deleting, the bot waits 30 seconds before proceeding to the next message.
5. **Repeat**: Once all messages have been sent and deleted, the process starts over from the first message.

## Setup Instructions

### Prerequisites
1. Install Python 3.x on your machine.
2. Install required dependencies:
   ```bash
   pip install requests pyyaml

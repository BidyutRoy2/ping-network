# Ping Network Auto Bot 🤖

An automated bot for the Ping Network VPN service to earn points and potentially qualify for airdrops.

## Features ✨

- Automated WebSocket connection to Ping Network
- Random zone selection for each session
- Dynamic User-Agent generation
- Analytics event tracking
- Automatic reconnection with exponential backoff
- Real-time points tracking
- Referral points monitoring

## Prerequisites 📋

- Node.js v16+
- npm/yarn
- Git

## Installation 🛠️

1. Clone the repository:
```bash
git clone https://github.com/BidyutRoy2/ping-network.git
cd ping-network
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file (or it will be auto-generated):

```
nano .env
```

```bash
USER_ID=  # Your Ping Network user ID
DEVICE_ID=     # Will be auto-generated if empty
```

## Usage 🚀

Start the bot:
```bash
npm start
```

The bot will:
- Generate a unique device ID if none exists
- Connect to Ping Network's WebSocket
- Send periodic analytics events
- Maintain connection with heartbeat pings
- Automatically reconnect if disconnected

## Configuration ⚙️

You can modify these values in `.env`:
- `USER_ID`: Your Ping Network user ID
- `DEVICE_ID`: Unique device identifier (auto-generated)

## Logging 📝

The bot provides color-coded console output:
- ✅ Success messages
- ⚠ Warning messages
- ✗ Error messages
- ⟳ Loading/process messages
- ➤ Step-by-step execution

Edward Admin Bot

A Telegram federation + global ban admin bot.

## 🚀 Docker Usage

### Build the image
```bash
docker build -t edward-admin .
```

### Run the container
```bash
docker run --rm \
  --env-file .env \
  -v $(pwd)/data:/data \
  edward-admin
```

Or use **Docker Compose**:
```bash
docker compose up -d
```

### Environment Variables
- `BOT_TOKEN` – Your Telegram bot token from [@BotFather](https://t.me/BotFather)

### Data Persistence
Bot state is stored in `/data/data.json`.  
Mount `./data` on the host to persist between restarts.

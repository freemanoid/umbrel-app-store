# Freemanoid's Umbrel app store

Personal [Umbrel community app store](https://github.com/getumbrel/umbrel-community-app-store).

Add it on your Umbrel: App Store → ⋯ → Community App Stores → paste this repo's URL.

## Apps

### TG Torrent Bot (`freemanoid-tg-torrent-bot`)

Headless Telegram bot: interactive torrent search via Prowlarr → download via
Transmission, plus filter-based subscriptions (auto-download new releases).
Image: `ghcr.io/freemanoid/tg-torrent-bot`, source: [freemanoid/tg-torrent-bot](https://github.com/freemanoid/tg-torrent-bot).

Configuration — the app expects `.env` in its app-data directory
(`~/umbrel/app-data/freemanoid-tg-torrent-bot/.env`):

```
TELEGRAM_TOKEN=...          # from @BotFather
ALLOWED_CHAT_ID=...         # your numeric Telegram user id
PROWLARR_URL=http://prowlarr_server_1:9696
PROWLARR_API_KEY=...
TRANSMISSION_URL=http://transmission_server_1:9091
```

SQLite state lives in `app-data/freemanoid-tg-torrent-bot/data/`.

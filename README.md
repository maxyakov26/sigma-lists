# sigma-lists

The Telegram Mini App page for managing the Yakov Alerts sigma lists. One static file, no build step,
served by GitHub Pages at `https://maxyakov26.github.io/sigma-lists/`.

- The page holds **no data**. The bot puts the current lists into the button link after `#` (compressed JSON);
  the page reads it, lets the user edit, and sends the changes back through Telegram (`sendData`). The bot
  validates and applies them.
- Opened outside Telegram it shows demo data and never sends anything.
- Spec: `tg-alert-bot/docs/WEB_LISTS_SPEC.md`.

Local check: open `index.html` in a browser (demo), or `index.html#s=<payload>` with a payload made by
`tg-alert-bot/scripts/sigma_payload.py`.

# Jonas by SimplifAId

Jonas is an email assistant for small businesses and busy people, made by SimplifAId in South Africa. Say "Hello Jonas" in a new chat and he sets himself up in a few simple questions. After that he tidies your Gmail every morning, sends you a short list of what needs you today, keeps a register of your receipts for tax, tells you who is waiting on a reply, and helps you look after your customers. He never sends an email without your clear yes.

Jonas needs a SimplifAId account: a free 14-day trial, then R250 a month. Sign up at https://simplifaid.online/start-trial.

## How it works

This plugin adds Jonas's skills (start, morning-summary, clean-up, receipts, reply-tracker and more) and the SimplifAId connector at https://simplifaid.online/mcp.

Each skill is a short pointer. When a skill runs, Claude calls the SimplifAId connector tool `get_jonas_job` with the skill's name, and the connector returns Jonas's current instructions and safety rules for that job. That way every customer always has the newest Jonas without installing anything again. The connector only returns instructions while the person's trial or subscription is active; otherwise it returns a short "Jonas is paused" message.

You sign in to the connector once, with the email address you signed up with and a one-time code we email you.

## What it runs, sends and fetches

- **Runs:** no local code. There are no scripts, hooks or binaries in this plugin.
- **Sends to SimplifAId:** your sign-in email address and the name of the Jonas job being run (for example `morning-summary`). Nothing else. Your email content, contacts and messages never go to SimplifAId.
- **Fetches from SimplifAId:** Jonas's written instructions for the job (plain text), through two read-only tools, `get_jonas_job` and `get_jonas_file`.
- **Uses in Claude:** your own Gmail and Google Calendar connectors, which you connect yourself. Jonas reads and tidies your mail there, inside your Claude account.
- **Public information Jonas looks up:** the weather for your town (Open-Meteo, open-meteo.com), local and business news headlines (Google News), coin prices if you ask for price alerts (CoinGecko, api.coingecko.com), and Claude's web search for news and job openings. Only a town name, a coin name or a search phrase goes out; never your emails, contacts or messages.
- **What Jonas keeps:** short notes about your setup and preferences, and your receipts list, saved in your own Claude workspace (or your own computer folder or Google Drive, if you choose). SimplifAId keeps only your sign-up email and your trial or subscription dates.

Privacy policy: https://simplifaid.online/privacy · Terms: https://simplifaid.online/terms

## Support

WhatsApp +27 74 063 8272, or see https://simplifaid.online/help.

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

Privacy policy: https://simplifaid.online/privacy · Terms: https://simplifaid.online/terms

## Support

WhatsApp +27 74 063 8272, or see https://simplifaid.online/help.

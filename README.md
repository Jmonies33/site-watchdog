# site-watchdog

Checks that the sites in `sites.txt` answer, every 30 minutes, from GitHub's servers.
A failed check fails the run (GitHub emails the owner). With the four Twilio secrets set
(`TWILIO_ACCOUNT_SID`, `TWILIO_API_KEY_SID`, `TWILIO_API_KEY_SECRET`, `ALERT_FROM`, `ALERT_TO`; a revocable API key, never the main auth token) it also texts once
when a site goes down and once when it comes back. No secrets live in this repository.

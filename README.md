# site-watchdog

Checks that the sites in `sites.txt` answer, every 30 minutes, from GitHub's servers.
A failed check fails the run (GitHub emails the owner). With the four Twilio secrets set
(`TWILIO_ACCOUNT_SID`, `TWILIO_AUTH_TOKEN`, `ALERT_FROM`, `ALERT_TO`) it also texts once
when a site goes down and once when it comes back. No secrets live in this repository.

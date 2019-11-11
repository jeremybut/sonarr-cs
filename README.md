# Sonarr-CS

Sonarr-CS is a custom script to send a notification to slack when sonarr download, upgrade or rename an episode.

## Installation

Clone this repo to your local machine using:

```bash
git clone https://gitlab.com/buttice.j/sonarr-cs.git
```

## Usage

**Go to `sonarr` > `Settings` > `Connect` > `Add Custom script`**

> Name `Named this script`

> On Grab `no`

> On Download `yes`

> On Upgrade `yes`

> On Rename `yes`

> Path `/where-the-script-is/main.py`

> Arguments `-wu https://hooks.slack.com/services/xxx/xxx/xxx -se http://localhost:8989/api -sk 8xxxxxxxxxxxxxxxxc -tk fxxxxxxxxxxxxxxxxxxxxxxxxxx5`

**Arguments explanation**

Slack webhook url, create it on `https://my.slack.com/services/new/incoming-webhook/`

> -wu https://hooks.slack.com/services/xxx/xxx/xxx

Sonarr API endpoint

> -se http://localhost:8989/api

Sonarr API key, find it on Sonarr > Settings > General

> -sk 8xxxxxxxxxxxxxxxxc

TMDB API Key, register app on tmdb to obtain API Key

> -tk fxxxxxxxxxxxxxxxxxxxxxxxxxx5

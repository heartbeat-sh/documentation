# Heartbeat.sh Documentation
Welcome to [heartbeat.sh](https://heartbeat.sh). The easiest way, by far, to set up your own heartbeat monitoring service.

## Why Heartbeat.sh?
[Heartbeat.sh](https://heartbeat.sh) is a free [heartbeat monitoring](https://en.wikipedia.org/wiki/Heartbeat_(computing)) tool, for proactively monitoring your servers and processes. Heartbeat monitoring makes it easy to monitor processes, especially ones that run on a cron. To automate operational checks, just send a heartbeat as part of your process. It's that easy!

## Getting Started
Create your own heartbeat server at [heartbeat.sh](https://heartbeat.sh). Enter a subdomain for your server, and click on create.

You can start sending your heartbeats right away. To send a heartbeat, just send a POST request to `/beat/{name}` on your server.
```
curl -X POST 'https://{subdomain}.heartbeat.sh/beat/{name}'
```
The server will reply with your heartbeat in JSON if everything worked okay. You can then navigate to `https://{subdomain}.heartbeat.sh` to see your heartbeat dashboard. The dashboard will show all your heartbeats and their states.

For more information, check out our [wiki](https://github.com/heartbeat-sh/documentation/wiki).
 
 ## Client Libraries
 
We aim to make heartbeat monitoring as easy as possible for developers. So we are working on client libraries for most popular programming languages. We currently have these available:

- [Bash Shell](https://github.com/heartbeat-sh/heartbeat.sh)
- [JavaScript](https://www.npmjs.com/package/heartbeat-sh)
- [Python](https://pypi.org/project/heartbeat-sh/)

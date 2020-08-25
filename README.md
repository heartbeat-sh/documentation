# Heartbeat.sh Documentation
Welcome to [heartbeat.sh](https://heartbeat.sh). The easiest way to set up heartbeat monitoring by far.

## Getting Started
Create your own heartbeat server at [heartbeat.sh](https://heartbeat.sh). Enter a subdomain for your server, and click on create.

You can start sending your heartbeats right away. To send a heartbeat, just send a POST request to `/beat/{name}` on your server.
```
curl -X POST 'https://{subdomain}.heartbeat.sh/beat/{name}'
```
The server will reply with `{name} at {date and time}, warning: 1m0s, error: 5m0s` if everything worked okay. You can then navigate to `https://{subdomain}.heartbeat.sh` to see your heartbeat dashboard. The dashboard will show all your heartbeats and their states.
 
 ## Client Libraries
 
 We aim to make heartbeat monitoring as easy as possible for developers. So we are working on client libraries for most popular programming languages. We currently have these available:

- [bash shell](https://github.com/heartbeat-sh/heartbeat.sh)
- [javascript](https://www.npmjs.com/package/heartbeat.sh)

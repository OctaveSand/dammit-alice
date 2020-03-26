# Dammit Alice v.01

Dammit-Alice is a discord api logger, which simply dumps all message-create traffic accessable to your user-token. It ignores deletes, so it's sure to catch those pesky users with a quick-trigger-delete finger. 

It requires a discord API token to run, which you can extract from your session (in chrome) by going to developer tools -> Network, and reading the Send headers on the "messages?limits=50" request. You're looking for the "Authorization" header. Once you have that, simply compile dammit-alice with a `go build` and run with `./ra -t <your-user-token>`

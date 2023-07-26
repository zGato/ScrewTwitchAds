# Mobile syntax

To use any of the proxies listed [here](proxies.md#proxies-list) you need to use a specific syntax depending on your modded app. You can use the following as reference:

To use all the proxies except `https://purpletv.cdn-perfprod.com` and `api.ttv.lol` with Twitch modded apps you need to specify in the address field the following: 
- `https://proxyaddress/live/$channel?allow_source=true&allow_audio_only=true&fast_bread=true` (Tested with Xtra app)

`$channel` is the variable for the channel name. Change it if your app uses other variable.

`?allow_source=true&allow_audio_only=true&fast_bread=true` are some variables asking for a playlist with those options available. Some apps may use them or more options and some others may not.


To use the `https://api.ttv.lol` proxy, you unfortunately need to modify the modded app source code if it doesn't have it available for you to choose. `api.ttv.lol` requires the `X-Donate-To` header and it can't be implemented without modifying the app source code. 


To use the `https://purpletv.cdn-perfprod.com` you need to specify the following in the address field: 
- `https://purpletv.cdn-perfprod.com/streamer/$channel` (Tested with Xtra app)

`$channel` is the variable for the channel name. Change it if your app uses other variable.

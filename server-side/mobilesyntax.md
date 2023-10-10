# Mobile syntax

To use any of the proxies listed [here](proxies.md#proxies-list) you need to use a specific syntax depending on your modded app. You can use the following as reference:

To use all the proxies with Twitch modded apps you need to specify in the address field the following: 
- `https://proxyaddress/live/$channel?allow_source=true&allow_audio_only=true&fast_bread=true` (Tested with Xtra app)
- `https://proxyaddress/live/$channelName` (Tested with PurpleTV app)

`proxyaddress` replace the proxy address with your own/from the list (ex: lb-eu.cdn-perfprod.com)

`$channel` & `$channelName` are the variables for the channel name. Change it if your app uses other variable.

`?allow_source=true&allow_audio_only=true&fast_bread=true` are some variables asking for a playlist with those options available. Some apps may use them or more options and some others may not.

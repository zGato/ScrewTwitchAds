# ScrewTwitchAds
Make sure to take a look at the main community repo [/pixeltris/TwitchAdSolutions](https://github.com/pixeltris/TwitchAdSolutions)

I've created this repo to add extra AdBlocking methods and change it a bit.

This repo consists in various ways to circumvent Twitch Ads, either client-sided solutions or server-sided.

# **DO NOT COMBINE TWITCH ADBLOCKERS!**
# **SERIOUSLY. DON'T COMPLAIN ABOUT IT NOT WORKING IF YOU USE MULTIPLE SIMULTANEOUSLY.**

# For desktop users
## [RECOMMENDED] Server-sided blocking methods

Proxies are usually the best and most reliable way to circumvent Twitch Ads. Either way, check the [downsides of proxies](https://wiki.cdn-perfprod.com/v1/must-read/proxies#proxies-downsides). 

- `TTV LOL PRO V2` - [chrome](https://chrome.google.com/webstore/detail/ttv-lol-pro/bpaoeijjlplfjbagceilcgbkcdjbomjd) / [firefox](https://addons.mozilla.org/addon/ttv-lol-pro/) / [code](https://github.com/younesaassila/ttv-lol-pro)
  - A fork of `TTV LOL` with most of the code rewritten with new ad blocking capabilities.
  - Removes `in-stream` ads. Use `uBlock Origin` for banner ads and others.
  - Works thanks to simple HTTP proxies. V1 proxies are not compatible!
  - Works for everyone. Released & updated recently.
  - More information at: https://wiki.cdn-perfprod.com/
- `TTV LOL PRO V1` - [code](https://github.com/younesaassila/ttv-lol-pro/tree/v1)
  - A fork of `TTV LOL` with improved UX and some newly added features.
  - Same ad blocking system as the original `TTV LOL` extension.
  - Proxy the initial streamer.m3u8 to grab an ad-free playlist from an ad-free country.
  - Removes `in-stream` ads. Use `uBlock Origin` for banner ads and others.
  - Doesn't work for everyone. If you use specific proxies results may vary. Choose one from the [following list](https://wiki.cdn-perfprod.com/v1/must-read/proxies#public-proxy-list) or [host your own](server-side/proxies.md#host-your-own-proxy).
  - **Not supported & deprecated. Not recommended for non-advanced users.**
  - More information at: https://wiki.cdn-perfprod.com/v/v1/

## Client-sided blocking methods

- `video-swap-new` - [ublock](https://github.com/pixeltris/TwitchAdSolutions/raw/master/video-swap-new/video-swap-new-ublock-origin.js) / [userscript](https://github.com/pixeltris/TwitchAdSolutions/raw/master/video-swap-new/video-swap-new.user.js) / [ublock (permalink)](https://raw.githubusercontent.com/pixeltris/TwitchAdSolutions/0b5ea5ed8959a6b4eb4c1ea406aaa56313c9c907/video-swap-new/video-swap-new-ublock-origin.js)
  - Uses the embed player during ads.
  - Quality is dropped to `360p` when ads are being played.
- `vaft` - [ublock](https://github.com/pixeltris/TwitchAdSolutions/raw/master/vaft/vaft-ublock-origin.js) / [userscript](https://github.com/pixeltris/TwitchAdSolutions/raw/master/vaft/vaft.user.js) / [ublock (permalink)](https://raw.githubusercontent.com/pixeltris/TwitchAdSolutions/0b5ea5ed8959a6b4eb4c1ea406aaa56313c9c907/vaft/vaft-ublock-origin.js)
  - The same as `video-swap-new` but attempts to get a clean stream faster (may suffer from more freezing / playback issues).

**For the sake of security it's recommended to use a permalink when using uBlock Origin (as permalinks do not auto update).**

`ublock` **and** `userscript` **scripts do auto update which could lead to having your data compromised if the main repository gets compromised.**

### [Applying a script (uBlock Origin)](https://github.com/pixeltris/TwitchAdSolutions#applying-a-script-ublock-origin)

- Navigate to the uBlock Origin Dashboard (the extension options)
- Under the `My filters` tab add `twitch.tv##+js(twitch-videoad)`.
- Under the `Settings` tab, enable `I am an advanced user`, then click the cog that appears. Modify the value of `userResourcesLocation` from `unset` to the full url of the solution you wish to use (if a url is already in use, add a space after the existing url). e.g. `userResourcesLocation https://raw.githubusercontent.com/pixeltris/TwitchAdSolutions/0b5ea5ed8959a6b4eb4c1ea406aaa56313c9c907/video-swap-new/video-swap-new-ublock-origin.js`
- To ensure uBlock Origin loads the script I recommend that you disable/enable the uBlock Origin extension (or restart your browser).

If you would like to remove the script, remove the twitch-videload filter and replace the script url to `unset`

# For mobile users
## [RECOMMENDED] Server-sided blocking methods

Proxies are usually the best and most reliable way to circumvent Twitch Ads. Either way, check the [downsides of proxies](https://wiki.cdn-perfprod.com/v1/must-read/proxies#proxies-downsides). 

- `Xtra for Twitch` - [f-droid](https://f-droid.org/packages/com.github.andreyasadchy.xtra/) / [code](https://github.com/crackededed/Xtra)
  - Twitch player for Android.
  - You can select your own custom proxy. You can [host your own](server-side/proxies.md#host-your-own-proxy) or choose one from the [following list](https://wiki.cdn-perfprod.com/v1/must-read/proxies#public-proxy-list).
  - Use the [following syntax](server-side/mobilesyntax.md) when using your own proxy or one from the list.
  - Alternatively you can also use standard HTTP proxies.
  - Partially broken in some regions for some users. 
- `PurpleTV` - [apk](https://purpletv.aeong.win/)
  - Modified Twitch Android app with added functionalities.
  - You can select your own custom proxy. You can [host your own](server-side/proxies.md#host-your-own-proxy) or choose one from the [following list](https://wiki.cdn-perfprod.com/v1/must-read/proxies#public-proxy-list).
  - Use the [following syntax](server-side/mobilesyntax.md) when using your own proxy or one from the list.
  - Code is private and some features are locked behind a paywall.
  - Partially broken in some regions for some users.
- `TwitchAdBlock` (for iOS) - [code](https://github.com/level3tjg/TwitchAdBlock)
  - Modified Twitch iOS app with added functionalities.
  - **You must be able to sideload ipas to your iOS device.**
  - By default, client-sided ad block mechanism is enabled. It may or may not work for you.
  - You can select your own **HTTP/m3u8** custom proxy. You may find some proxies provided by their maintainer [here](https://github.com/level3tjg/TwitchAdBlock/releases/tag/v23.4-0.1.5), or use any from the [following list](https://wiki.cdn-perfprod.com/v1/must-read/proxies#public-proxy-list).
  - Alternatively, you can [host your own proxy](server-side/proxies.md#host-your-own-proxy).

# Developers

[Host your own proxy](server-side/proxies.md#host-your-own-proxy)

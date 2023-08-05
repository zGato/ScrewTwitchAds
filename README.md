# ScrewTwitchAds
The main repo which the community is usually told to go is [/pixeltris/TwitchAdSolutions](https://github.com/pixeltris/TwitchAdSolutions)

I've created this repo to add extra AdBlocking methods and change it a bit.

This repo consists in various ways to circumvent Twitch Ads, either client-sided solutions or server-sided.

**DO NOT COMBINE TWITCH ADBLOCKERS!**

# For desktop users
## [RECOMMENDED] Server-sided blocking methods

Proxies are usually the best and most reliable way to circumvent Twitch Ads. Either way, check the [downsides of proxies](server-side/proxies.md#proxies-downsides). 

- `TTV LOL PRO V2` - [chrome](https://chrome.google.com/webstore/detail/ttv-lol-pro/bpaoeijjlplfjbagceilcgbkcdjbomjd) / [firefox](https://addons.mozilla.org/addon/ttv-lol-pro/) / [code](https://github.com/younesaassila/ttv-lol-pro)
  - A fork of `TTV LOL` with most of the code rewritten with new ad blocking capabilities.
  - Removes `in-stream` ads. Use `uBlock Origin` for banner ads and others.
  - Works thanks to simple HTTP proxies. V1 proxies are not compatible!
  - Works for everyone. Released & updated recently.
- `TTV LOL PRO V1` - [code](https://github.com/younesaassila/ttv-lol-pro/tree/v1)
  - A fork of `TTV LOL` with improved UX and some newly added features.
  - Same ad blocking system as the original `TTV LOL` extension.
  - Proxy the initial streamer.m3u8 to grab an ad-free playlist from an ad-free country.
  - Removes `in-stream` ads. Use `uBlock Origin` for banner ads and others.
  - Doesn't work for everyone. If you use specific proxies results may vary. Choose one from the [following list](server-side/proxies.md#proxies-list) or [host your own](server-side/proxies.md#host-your-own-proxy).
- `TTV LOL` - [chrome](https://chrome.google.com/webstore/detail/ttv-lol/ofbbahodfeppoklmgjiokgfdgcndngjm) / [code](https://github.com/TTV-LOL/extensions)
  - Proxy the initial streamer.m3u8 to trab an ad-free playlist from an ad-free country.
  - Removes `in-stream` ads. Use `uBlock Origin` for banner ads and others.
  - Doesn't work for everyone. Locked to their own API. Proxy cannot be changed unless code is modified by yourself.

## Client-sided blocking methods

- `screwtwitchads` - [instructions](client-side/screwtwitchads.md) (**NOT RELEASED CURRENTLY**)
  - This does not involve continuously proxying (only first time for specific countries)
  - When ads are played, **there is no quality drop**
  - This system is experimental and may not work for everyone.
  - *basically same as having Twitch Turbo*
- `vaft` - [ublock](https://github.com/pixeltris/TwitchAdSolutions/raw/master/vaft/vaft-ublock-origin.js) / [userscript](https://github.com/pixeltris/TwitchAdSolutions/raw/master/vaft/vaft.user.js) / [ublock (permalink)](https://github.com/pixeltris/TwitchAdSolutions/raw/2bfda1e1a1c55d7b2dd4a541242acb5033644237/vaft/vaft-ublock-origin.js)
  - Modified `VAFT` original script which dropped resolution to `480p` when ads were played. Twitch patched it.
  - Now quality is dropped to `360p` when ads are being played.
  - Should work for everyone.

# For mobile users
## [RECOMMENDED] Server-sided blocking methods

Proxies are usually the best and most reliable way to circumvent Twitch Ads. Mobile platforms still use the streamer.m3u8 proxy method as it works for them (due to not having stitched ads). Either way, check the [downsides of proxies](server-side/proxies.md#proxies-downsides). 

- `Xtra for Twitch` - [f-droid](https://f-droid.org/packages/com.github.andreyasadchy.xtra/) / [code](https://github.com/crackededed/Xtra)
  - Modified Twitch app with added functionalities.
  - You can select your own custom proxy. You can [host your own](server-side/proxies.md#host-your-own-proxy) or choose one from the [following list](server-side/proxies.md#proxies-list).
  - Use the [following syntax](server-side/mobilesyntax.md) when using your own proxy or one from the list.
  - Works for everyone.
- `PurpleTV` - [apk](https://purpletv.aeong.one/)
  - Modified Twitch app with added functionalities.
  - You're locked to using their own provided list of proxies.
  - "Open source code". You need to request access to it, and only if you're a developer.
  - Works for everyone.

# Developers

[Host your own proxy](server-side/proxies.md#host-your-own-proxy)

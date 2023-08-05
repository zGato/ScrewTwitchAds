# Proxies downsides

You need to assume that if you use some other user's infrastructure, you're accepting that required maintenance and proxy downtime may occur. You may want to go by the [host your own](#host-your-own-proxy) route. 
Mobile platforms use the initial streamer.m3u8 ad block system, thus making that once you get the first request done, you no longer need that proxy working unless you switch between streamers. TTV LOL PRO V2 for example uses HTTP proxies, and it is required to have the server running all the time to not have buffering issues, thus making it much costly.

Consider giving your support by covering some of their infrastructure costs via donations if you feel they do a great job. You would have to pay 12€ / month to Twitch if amazing people in the community didn't spend their time looking for circumventions.

# Proxies list
## m3u8 proxies (Mobile users, TTV LOL PRO V1 and TTV LOL compatible)

- `https://api.ttv.lol` - [maintainer](https://ttv.lol/)
  - Proxied to multiple countries.
  - `X-Donate-To = "https://ttv.lol/donate` header required for the API to give successful requests.
- `https://lb-eu.cdn-perfprod.com` - [maintainer](https://github.com/zGato) / [current status](https://status.perfprod.com)
  - Proxied to the Netherlands.
  - Recommended for Desktop & Mobile users.
- `https://lb-eu2.cdn-perfprod.com` - [maintainer](https://github.com/zGato) / [current status](https://status.perfprod.com)
  - Proxied to Ukraine, Azerbajian and the Netherlands.
  - Recommended for Desktop & Mobile users.
- `https://lb-eu3.cdn-perfprod.com` - [maintainer](https://github.com/zGato) / [current status](https://status.perfprod.com)
  - Proxied to Russia.
  - Recommended for Mobile users.
- `https://lb-na.cdn-perfprod.com` - [maintainer](https://github.com/zGato) / [current status](https://status.perfprod.com)
  - Proxied to the US and Canada.
  - Not recommended at all. May or may not work.
- `https://lb-as.cdn-perfprod.com` - [maintainer](https://github.com/zGato) / [current status](https://status.perfprod.com)
  - Proxied to Singapore.
  - Recommended for Desktop & Mobile users.
- `https://eu.luminous.dev` - [maintainer](https://github.com/AlyoshaVasilieva) / [current status](https://stats.uptimerobot.com/N2pVRCZAjg)
  - Proxied to Lithuania.
  - Recommended for Mobile users.
- `https://eu2.luminous.dev` - [maintainer](https://github.com/AlyoshaVasilieva) / [current status](https://stats.uptimerobot.com/N2pVRCZAjg)
  - Proxied to Lithuania.
  - Recommended for Mobile users.
- `https://as.luminous.dev` - [maintainer](https://github.com/AlyoshaVasilieva) / [current status](https://stats.uptimerobot.com/N2pVRCZAjg)
  - Proxied to China.
  - Recommended for Desktop & Mobile users.
- `https://purpletv.cdn-perfprod.com` - [maintainer](https://t.me/nopbreak)
  - Proxied to Russia.
  - Recommended & only compatible for Mobile users.

# Host your own proxy

[Check out this tutorial](https://github.com/younesaassila/ttv-lol-pro/discussions/151) to create your own **HTTP** proxy

[Check out this project](https://github.com/AlyoshaVasilieva/luminous-ttv) to host your own **m3u8** proxy
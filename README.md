<div align="center">

<kbd>
<img style="border-radius:50%" height="150px" src="https://raw.githubusercontent.com/FogNetwork/Tsunami/main/public/img/logo.svg">
</kbd>

<h1>Tsunami</h1>

<h3>An official Fog Network proxy site, made to access the blocked web</h3>

<p>Surf without web filters or restrictions. Made with style, Tsunami is a rather fancy service dedicated to protecting your freedom from censorship.
Read the documentation below to find out more</p>

<p>Want to improve Tsunami? <a href="https://github.com/FogNetwork/Tsunami/compare">Create a pull request</a></p>
</div>

<p align="center">
<a href="https://heroku.com/deploy?template=https://github.com/FogNetwork/Tsunami"><img height="30px" src="https://raw.githubusercontent.com/FogNetwork/Tsunami/main/deploy/heroku2.svg"><img></a>
<a href="https://repl.it/github/FogNetwork/Tsunami"><img height="30px" src="https://raw.githubusercontent.com/FogNetwork/Tsunami/main/deploy/replit2.svg"><img></a>
<a href="https://glitch.com/edit/#!/import/github/FogNetwork/Tsunami"><img height="30px" src="https://raw.githubusercontent.com/FogNetwork/Tsunami/main/deploy/glitch2.svg"><img></a>
</p>

## Documentation

- [Overview](#overview)
  - [Supported Sites](#supported-sites)
  - [Features](#features)
  - [Pages](#pages)
- [Setup](#setup)
  - [Locally](#locally)
  - [Deploy](#deploy)
  - [Proxies](#proxies)
  - [Configuration](#configuration)
- [Support](#support)
  - [FAQ](#faq)
  - [Contact](#contact)
- [More](#more)
  - [Proxy Sources](#proxy-sources)
  - [Credits](#credits)
  - [Contributing](#contributing)

## Overview

### Supported Sites

- google.com
- discord.com
- youtube.com
- invidio.us
- reddit.com
- wolframalpha.com
- 1v1.lol
- schoolcheats.net?

### Features

- All the best proxies
- Nice game library
- Chatbox connected to discord
- Tab cloaking and other cool features
- Basic auth
- Customizable CSS
- Looks good

## Pages

- `/` Homepage
- `/1` Arcade
- `/2` Chatbox
- `/3` Settings
- `/4` Terms
- `/5` Privacy
- `/6` Documentation
- `/7` Credits
- `/8` Support and Contact
- `/404` 404 Error

## Setup

**Please Note: Womginx and PyDodge will not work without deploying are hosted on subdomains, see [proxies](#proxies) for more info**

### Locally

```sh
git clone https://github.com/FogNetwork/Tsunami

cd Tsunami

npm install

npm start
```

### Deploy

Click one of the buttons above and follow the steps

### Proxies

Some of the proxies on Tsunami are hosted on subdomains, deploy the correct proxy for Tsunami to work

Smoke and Corrosion are hosted locally, so you don't need a subdomain

[w.example.com (Womginx)](https://github.com/binary-person/womginx)

[p.example.com (PyDodge)](https://github.com/BinBashBanana/PyDodge)

[Locally (Smoke)](https://github.com/FogNetwork/Smoke)

[Locally (Corrosion)](https://github.com/titaniumnetwork-dev/Corrosion)

### Configuration

**config.json**

```json
{
    "port": "8080",
    "lite": "false",
    "auth": "false",
    "username": "user",
    "password": "secret"
}
```

`"port": "8080"` Changes the port 

`"lite": "false"` Hides Womginx and PyDodge, set to true or false 

`"auth": "false"` Basic authentication, set to true or false

`"username"` Username for authentication

`"password"` Password for authentication

**/public/js/go.js**

```js
var smokeproxy = window.location.protocol + "//" + window.location.hostname + "/smoke/gateway?url="

var corrosionproxy = window.location.protocol + "//" + window.location.hostname + "/corrosion/gateway?url="

var womginxproxy = window.location.protocol + "//" + "w." + window.location.hostname + "/main/"

var pydodgeproxy = window.location.protocol + "//" + "p." + window.location.hostname + "/course/"
```
`smokeproxy` Location for Smoke proxy

`corrosionproxy` Location for Corrosion proxy

`womginx` Location for Womginx proxy

`pydodgeproxy` Location for PyDodge proxy

Custom Proxy Example:

```js
var smokeproxy = "https://example.com/smoke/"
```

**/public/js/game.js**

```js
var corrosionproxy = window.location.protocol + "//" + window.location.hostname + "/corrosion/gateway?url="
```

`corrosionproxy` Location for game proxy

## Support

### FAQ

**How can I get new domains?**

Join our [discord](https://discord.gg/yk33HZSZkU) for more Tsunami links

**Captcha not working/issues**

Captcha is only supported on Womginx, though the support is limited

**Why is Discord not working properly?**

Try using Womginx or Corrosion. Refreshing the page might help

### Contact

Nebelung - [Nebelung#1335](https://discord.com/users/887118260963782686)

## More

### Proxy Sources

[Smoke](https://github.com/FogNetwork/Smoke)

[Corrosion](https://github.com/titaniumnetwork-dev/Corrosion)

[Modified Corrosion](https://github.com/BinBashBanana/Corrosion-Heroku)

[Womginx](https://github.com/binary-person/womginx)

[PyDodge](https://github.com/BinBashBanana/PyDodge)

[Alloy](https://github.com/titaniumnetwork-dev/alloy) (Not Used)

[SystemYA](https://github.com/sysce/proxy) (Not Used)

[Via](https://github.com/hypothesis/via) (Not Used)

[Node Unblocker](https://github.com/nfriedly/node-unblocker) (Not Used)

[Powermouse](https://github.com/titaniumnetwork-dev/powermouse) (Not Used)

### Credits

[Nebelung](https://github.com/Nebelung-Dev) - Owner and Main Developer

[EnderKingJ](https://github.com/EnderKingJ) - Proxy Developer

[Quite A Fancy Emerald](https://github.com/QuiteAFancyEmerald) - Holy Unblocker King

[Caracal.js](https://github.com/caracal-js) - Proxy Developer

[MikeLime](https://github.com/MikeLime-dev) - Developer

[BinBashBanana](https://github.com/BinBashBanana) - Game Library and PyDodge 

[Binary Person](https://github.com/binary-person) - Creator of Womginx

[Divide](https://github.com/vibedivide) - SystemYA and Chatbox Creator

[Shirt](https://github.com/shirt-dev) - Proxy Developer

[Karlee Rae](https://github.com/KarleeRae) - MinecraftJS

### Contributing

See [CONTRIBUTING.md](https://github.com/FogNetwork/Tsunami/blob/main/CONTRIBUTING.md)

Special Thanks Quite A Fancy Emerald, Inspiration for Tsunami

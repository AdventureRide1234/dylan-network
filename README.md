# Incognito
Access the world wide web!



## Setup

```sh
git clone https://github.com/titaniumnetwork-dev/Incognito
cd Incognito
npm install
npm start
```

## Config

```json
{
    "port": 8080,
    "ssl": false,
    "prefix": "/service/",
    "codec": "xor",
    "proxy": true,
    "blacklist": [],
    "addresses": [],
    "authorization": {
        "name": "__incog_auth",
        "value": "1"
    },
    "appearance": "bright",
    "engine": "google"
}
```

- `port` HTTP Server Port
- `ssl` (true / false) HTTP Server SSL
- `prefix` Corrosion proxy prefix
- `codec` Corrosion proxy codec
- `proxy` (true / false) Have Corrosion be hosted on the Node.js application. Recommended to have Corrosion hosted elsewhere with large amounts of clients.
- `blacklist` Array of hostnames to be blocked on the proxy.
- `authorization` (Object { name: "...", value: "..." } / false) Proxy authorization cookie
- `appearance` ("bright" / "midnight" / "ocean" / "lime" / "terminal") Default site appearance
- `engine` ("google" / "bing" / "brave" / "youtube" / "twitter" / "reddit") Default search engine 


## Games

More games can be added to Incognito by adding JSON in `gs.json` in a specific format.
```json

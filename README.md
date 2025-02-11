# AmnewziaWG Easy

You have found the easiest way to install & manage AmneziaWG on any Linux host!

<p align="center">
  <img src="https://github.com/spcfox/amnezia-wg-easy/raw/master/assets/screenshot.png" width="802" />
</p>

## Features

* All-in-one: AmneziaWG + Web UI.
* Easy installation, simple to use.
* List, create, edit, delete, enable & disable clients.
* Download a client's configuration file.
* Statistics for which clients are connected.
* Tx/Rx charts for each connected client.
* Gravatar support.
* Automatic Light / Dark Mode
* Multilanguage Support
* UI_TRAFFIC_STATS (default off)

## Requirements

* A host with Docker installed.

## Settings
All settings are stored in an .env file, below is a description of each line.

| Env | Default | Example | Description |
| - | - | - | - |
| `WG_HOST` | - | `vpn.myserver.com` | The public hostname of your VPN server. |
| `LANGUAGE` | `en` | `de` | Web UI language (Supports: en, ru, tr, no, pl, fr, de, ca, es). |
| `PORT` | `51821` | `6789` | TCP port for Web UI. |
| `WG_DEFAULT_ADDRESS` | `10.8.0.x` | `10.6.0.x` | Clients IP address range. |
| `WG_DEFAULT_DNS` | `1.1.1.1` | `8.8.8.8, 8.8.4.4` | DNS server clients will use. If set to blank value, clients will not use any DNS. |
| `WG_ALLOWED_IPS` | `0.0.0.0/0, ::/0` | `192.168.15.0/24, 10.0.1.0/24` | Allowed IPs clients will use. |
| `PASSWORD` | - | `foobar123` | When set, requires a password when logging in to the Web UI. |
| `PASSWORD_HASH` | - | `$2a$12$e.ywzeb6ZcQ6nf21ZxEFb.6D.VxnLSTQjIYKqEXFZoWtI2W/bSqMS` | When set, requires a password when logging in to the Web UI. Get hash: docker run -it ghcr.io/w0rng/amnezia-wg-easy wgpw YOUR_PASSWORD |

## Thanks

Based on [wg-easy](https://github.com/wg-easy/wg-easy) by Emile Nijssen.

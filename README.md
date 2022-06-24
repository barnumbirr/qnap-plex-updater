# qnap-plex-updater

Shell script aimed at updating Plex Media Server on QNAP servers.

## Prerequisites:

- Entware [installed on your device](https://github.com/Entware/entware/wiki/Install-on-QNAP-NAS)
- `git` installed


## Installation

Clone the repository:

```bash
$ cd /opt/
$ git clone https://github.com/barnumbirr/qnap-plex-updater.git
$ cd qnap-plex-updater
$ chmod +x bin/qnap-plex-updater
```

## Usage

### Manual

```bash
[~] # /opt/qnap-plex-updater/bin/qnap-plex-update --channel public
Downloading Plex Media Server 1.26.2.5797-5bd057d2b-x86_64...
Installing and restarting Plex Media Server...
Plex Media Server 1.26.2.5797-5bd057d2b-x86_64 installed successfully!
[~] #
```

### Cron job schedule

```bash
$ echo "30 1 * * * /opt/qnap-plex-updater/bin/qnap-plex-updater --channel public > /dev/null 2>&1" >> /etc/config/crontab
$ crontab /etc/config/crontab && /etc/init.d/crond.sh restart
```

## License:

```
Copyright 2022 Martin Simon

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## Buy me a coffee?

If you feel like buying me a coffee (or a beer?), donations are welcome:

```
BTC : bc1qq04jnuqqavpccfptmddqjkg7cuspy3new4sxq9
DOGE: DRBkryyau5CMxpBzVmrBAjK6dVdMZSBsuS
ETH : 0x2238A11856428b72E80D70Be8666729497059d95
LTC : MQwXsBrArLRHQzwQZAjJPNrxGS1uNDDKX6
```

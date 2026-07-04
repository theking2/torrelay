# torrelay

Tor relay with docker / docker compose

## Prerequisities

* You need docker / docker compose installed on a linux machine with amd64 architecture.
* You should know what tor and tor relays are.
* You should know what You are doing.

## Getting Started

#### configure torrc

* Copy torrc.EXAMPLE to torrc
* Change Nickname and ContactInfo
* If running multiple relays, uncomment MyFamily line and insert relay info
* Check and adjust ORPort, BandwidthRate, MaxAdvertisedBandwidth, MaxMemInQueues
* (Or use your own torrc)

#### configure compose.yaml

* Check and adjust compose.yaml
* run ``docker compose up -d && docker compose logs -f`` to start the relay and check the logs 

## Volumes

* `/etc/tor/torrc` - torrc
* `/var/lib/tor` - tor data directory

## GitHub repository
* [Github](https://github.com/theking2/torrelay/)

## Acknowledgments

* This project is inspired by [docker-obfs4-bridge](https://gitlab.torproject.org/tpo/anti-censorship/docker-obfs4-bridge)

[![Build Status](https://travis-ci.org/infiniteproject/icecast.svg?branch=master)](https://travis-ci.org/infiniteproject/icecast)
# icecast
Icecast 2 for Docker
```
docker run -d -p 8000:8000 --env-file .env icecastrelay:latest
docker run --rm -it -v "/tmp/:/var/log/icecast"  -p 8000:8000/tcp --env-file .env icecastrelay:latest
```
Supported ENV variables:

```
ICECAST_SOURCE_PASSWORD, ICECAST_ADMIN_PASSWORD, ICECAST_RELAY_PASSWORD
ICECAST_ADMIN_USERNAME, ICECAST_ADMIN_EMAIL
ICECAST_LOCATION, ICECAST_HOSTNAME
ICECAST_MAX_CLIENTS, ICECAST_MAX_SOURCES, MASTER_SERVER, MASTER_SERVER_PORT,
MASTER_UPDATE_INTERVAL, MASTER_PASSOWRD, RELAYS_ON_DEMAND
```

# Docker Status

Eseguire questo comando nella macchina su cui è installato Docker per sapere che tutto è ok

```
$ curl https://get.javanile.org/docker-status | sudo bash -
```

## Status Checks

- Verificare che docker-compose up -d funzioni su un progette creato al volo sulla cartella /tmp e poi rimosso dopo il test
- Verificare la presensa sia di "docker compose" che "docker-compose"

## Problems & Solutions

Problem

```
Cannot autolaunch D-Bus without X11 $DISPLAY
```

Solution

```
dpkg -r --ignore-depends=golang-docker-credential-helpers golang-docker-credential-helpers
```

Reference

- https://stackoverflow.com/questions/51222996/docker-login-fails-on-a-server-with-no-x11-installed

# Docker Status

Eseguire questo comando nella macchina su cui è installato Docker per sapere che tutto è ok

```
$ curl https://get.javanile.org/docker-status | sudo bash -
```

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

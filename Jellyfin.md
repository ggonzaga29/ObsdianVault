# Scripts for Jellyfin

Jellyfin.sh
```bash
#!/bin/sh
DISKDRIVE="/run/media/gian/1C40702F1049ECF4/"

while [ ! -d "$DISKDRIVE" ]; do
    sleep 10
done

setfacl -m "g:jellyfin:rwx" /run/media/gian
systemctl start jellyfin.service

```

jellyfin.service
```
[Unit]
Description=Activate permission for jellyfin

[Service]
ExecStart=/home/gian/jellyfin.sh

[Install]
WantedBy=multi-user.target

```
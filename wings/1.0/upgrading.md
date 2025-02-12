# Upgrading Wings
Upgrading Wings is a painless process and should take less than a minute to complete.

## Download Updated Binary
First, download the updated wings binary into `/usr/local/bin`.

::: warning
`Wings@1.2.0` requires `Panel@1.2.0` in order to run properly.
:::

``` bash
curl -L -o /usr/local/bin/wings https://github.com/pterodactyl/wings/releases/download/v1.2.0/wings_linux_amd64
chmod u+x /usr/local/bin/wings
```

## Restart Process
Finally, restart the wings process. Your running servers will not be affected and any open
connections to the instance will re-connect automatically.

``` bash
systemctl restart wings
```

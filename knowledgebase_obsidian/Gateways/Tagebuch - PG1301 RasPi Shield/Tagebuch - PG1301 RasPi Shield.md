## Fragen

## Aufgetretene Probleme

_WICHTIG: Library/Service von Dragino für das Shield funzt nur mit 32 bit OS!_

## Tagebuch

### Inbetriebnahme

- Neues Raspi OS mit
  - Hostname: `pg1301-hfu.local`
  - Passwort: `Darkened;Previous3;Contrite;Monkhood`
  - WLAN Config für `Vladimir Routin` zuhause, fürs Erste

### Konfiguration

- Laut Manual: Gateway EUI ist MAC der eth0-Schnittstelle des Pi mit `ffff`-Suffix: `  e45f015c9d5effff `
- SPI in `raspi-config` aktivieren
- Herunterladen des Pakets mit `wget http://www.dragino.com/downloads/downloads/LoRa_Gateway/PG1301/software/lorapktfwd.deb`
- Dann Installation mit `sudo dpkg -i lorapktfwd.deb`
- Für einfachere Bearbeitung der config-files verwende VS Code Remote Development mit SSH
- `/etc/lora-gateway/local_conf.json`: Konfiguration reinschreiben, z.B.:

```json
{
    "gateway_conf": {
        "gateway_ID": "E45F015C9D5EFFFF",
        "server_address": "eu1.cloud.thethings.network"
    }
}
```

### Neustarten des Service

`sudo systemctl stop lorapktfwd`
`sudo systemctl start lorapktfwd`
...oder einfach `sudo systemctl restart lorapktfwd`
Zum Überprüfen des Status: `sudo systemctl status lorapktfwd`

### Verbindung zu TTN erfolgreich

- Danach erscheint das Gateway als aktiv auf TTN!
- => <https://eu1.cloud.thethings.network/api/v3/gateways/eui-e45f015c9d5effff>

## TODO

- GPS geht noch nicht

## Life Lessons

Yay, das Paket ist 32bit, nicht 64bit :)))))
![[Pasted image 20230224185357.png]]

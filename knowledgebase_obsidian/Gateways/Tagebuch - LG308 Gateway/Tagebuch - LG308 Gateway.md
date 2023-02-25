## Eckdaten

- Gateway EUI: A840412032B04149

## Aufgetretene Fehler

### BLOCKER: Gateway ist schon/noch registriert?

```json
{
  "code": 6,
  "message": "error:pkg/identityserver:gateway_eui_taken (a gateway with EUI `A840412032B04149` is already registered (by you or someone else) as `a840412032b04149`)",
  "details": [
    {
      "@type": "type.googleapis.com/ttn.lorawan.v3.ErrorDetails",
      "namespace": "pkg/identityserver",
      "name": "gateway_eui_taken",
      "message_format": "a gateway with EUI `{gateway_eui}` is already registered (by you or someone else) as `{gateway_id}`",
      "attributes": {
        "administrative_contact": "hfuserhat",
        "gateway_eui": "A840412032B04149",
        "gateway_id": "a840412032b04149"
      },
      "correlation_id": "faf8bd241556454bba4c7727db8872f8",
      "code": 6
    }
  ]
}
```

Siehe auch: <https://eu1.cloud.thethings.network/api/v3/gateways/a840412032b04149>

ggf. Cochlovius fragen, ob er es bei sich rauswerfen kann bzw. ob der Account noch existiert?

## Fragen

- Was heißt "LoRaWAN 'Pico' Gateway"?
- Was ist ein LoRa Concentrator?
- Verbindet sich ein Gateway auch automatisch mit anderen Gateways im LoRaWAN-Netzwerk oder geht die Verbindung zu anderen Gateways nur per Ethernet/WLAN?

## Anmerkungen

- Verwendet wohl auch den Semtech Packet Forwarder, wie ihn Z. auch i seiner Mail erwähnt hat
  - <https://www.thethingsindustries.com/docs/gateways/concepts/udp/>

## "Logbuch"

### Funktionsweise im Netzwerk

![[Pasted image 20230224142358.png]]

### System overview

![[Pasted image 20230224142347.png]]

### Einrichtung

- Verbindung mit Laptop zum WLAN-AP des Gateways mit dem Namen `dragino-xxxxxx`
  - Standard-Passwort: `dragino+dragino`
- Aufruf der IP-Adresse `10.130.1.1` im Browser zum Zugriff auf Konfigurations-Webinterface
- Standard-Credentials für Web-Interface
  - User: `root`
  - PW: `dragino`
- Verbindung per Ethernet und WLAN tut auch

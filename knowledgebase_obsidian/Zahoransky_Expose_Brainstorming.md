# Zahoransky Thesis Exposé - Standortbestimmung mit LoRa auf Basis des `The Things Network`

## "Vorhaben" beschreiben

## "Warum ist das interessant?"

- Lokalisierung über LoRa ist interessant, da keine GPS- oder WLAN-Antenne vorhanden sein muss
  - LoRa kann so eine grobe Positionsbestimmtung durchfüühren sowie Daten übertragen

## Papers

- <https://ieeexplore.ieee.org/document/9289280>
- <https://www.mdpi.com/2078-2489/13/6/303>

## Methodik

- API von The Things Network querien, um Standorte von Gatways zu erhalten
- Voronoi-Diagramme zum Interpolieren von fehlenden Messungen anlegen
- Geht auch TOF MEssung?
	- Je nachdem, wie genau die Zeitstempel von TTN sind

## Zeitplan

- 1.9.23: Exposé abgeben

## Interessante Links

- [The Things Network](https://www.thethingsnetwork.org/)
  - <https://www.thethingsnetwork.org/docs/devices/node/map/>
- <https://www.youtube.com/watch?v=SxSXJxE07dE>
- <https://www.thethingsindustries.com/docs/integrations/lora-cloud/geolocation/>
  - <https://www.loracloud.com/documentation/geolocation?url=v3.html>
    - Gibt's basically schon? :(

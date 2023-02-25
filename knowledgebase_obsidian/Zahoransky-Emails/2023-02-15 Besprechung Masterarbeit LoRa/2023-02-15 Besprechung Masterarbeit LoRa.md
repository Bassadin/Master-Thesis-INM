Hallo Herr Hodapp,

hier ist noch etwas mehr Dokumentation zum Semtech Packet Forwarder, den Sie für das Raspi-Shield benötigen:

<https://www.thethingsnetwork.org/docs/gateways/packet-forwarder/semtech-udp/> (für eine ältere Version von TTN)

<https://www.thethingsindustries.com/docs/gateways/concepts/udp/> (für die aktuelle Version von TTN)

Konfiguriert wird das LoRaShield über eine Config-Datei. Hier muss angegebene werden, an welchen Server die einkommenden LoRa Nachrichten weitergeleitet werden sollen. Für TTN ist das eu1.cloud.thethings.network. Anbei finden Sie eine Konfigurationsdatei, die (zumindest) für mein Gateway funktioniert. Die ID meines Gateways habe ich entfernt. Sie müssen hier Ihre eigene ID eintragen. Die ID wird von TTN generiert oder von Ihnen festgelegt, wenn Sie ein neues Gateway in der TTN Konsole erstellen.

Jetzt habe ich zwei weitere Gateways, die ich Ihnen zur Verfügung stellen kann. Das können wir gerne Anfang März machen. Oder, falls Sie wollen: Versuchen Sie mich anzurufen, dann kann ich Ihnen die Hardware auch jetzt noch geben (nur wenn Sie wollen).

Zur TTNMapper API: Es gibt die Möglichkeit alle von einem Gateway empfangenen Signale als CSV ausgeben zu lassen: <https://ttnmapper.org/gateways/csv.html?gateway=Innolab-RAKete&startdate=2020-02-15&enddate=2023-02-15> zeigt alle Einträge zum Gateway „Innolab-RAKete“ zwischen dem 15.02.2020 und 15.02.2023. So können Sie irgendwann über alle Ihre Gateways iterieren und sich selbst eine Datenbank aufbauen.

Genauso können Sie für einen einzelnen Tracker ausgeben lassen, was aufgezeichnet wurde: <https://ttnmapper.org/devices/csv.html?device=blinkeding&startdate=2023-02-10&enddate=2023-02-15> zeigt für den Tracker „Blinkeding“ wo er sich befunden hat und welche Gateways das Signal empfangen haben.

<https://ttnmapper.org/advanced-maps/> ist die „GUI“ dazu.

Viele Grüße

R. Zahoransky

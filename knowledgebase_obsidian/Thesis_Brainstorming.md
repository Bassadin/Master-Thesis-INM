# Brainstorming für Master-Thesis Sommersemester 2023

## Professorenspezifisch

### Prof. Zahoransky

- Smart Home
  - Matter
    - Bestehendes Gerät in Matter einbinden
      - ESP32 so programmieren, dass er mit Matter funktioniert und auch mit Home Assistant kommuniziert
        - Matter-Spezifikation lesen, etc.
        - Einbindung in Matter-Netzwerk und Auslesen von Daten über Home Assistant
        - Matter ist eine aktuelle Technologie und es gibt noch nicht viel Forschung
          - Risiko: Noch nicht viele Quellen
          - Aber: Offener Standard, potenziell große Zukunftsrelevanz
            - Unterstützt von vielen Unternehmen wie Google, Amazon, Apple, etc.
  - Home Assistant

- Wireless Tech
  - LoRa
  - LoRaWAN
    - Repeater für LoRa-Stationen
      - Risiko: Nicht viel Low-Level Expertise vorhanden
  - Empfangsstärken mit Voronoi-Interpolation oder Area-Based-Probability
    - Verbindung mit TTN
    - Voronoi-Diagrammen zum Interpolieren von fehlenden Messungen
  - Lokalisierung per LoRa
    - Karte aufbauen mit GPS-Empfänger und dann auf der TTN-Karte die Positionen der LoRa-Stationen eintragen und abgleichen
      - vllt noch kombinieren mit WLAN?
      - Sensoren triangulieren auf der TTN-Map?

- Exposé (2 Seiten) - "Lokalisierungsmöglichkeiten mit LoRa"
  - "Vorhaben" beschreiben
  - "Warum ist das interessant?"
    - Lokalisierung über LoRa ist interessant, weil man keine GPS- oder WLAN-Antenne hat
    - TTNMapper-Karte ist "gratis" -> "Crowdfunding"
  - Paper raussuchen
  - Methodik
  - Zeitplan

### Prof. Piepmeyer

- Abgeben bis zum 1.3.2023 und unterschreiben lassen

- Scala

- Datenbanken
  - MongoDB

- Webentwicklung
  - Frameworks
    - Vue.js
  - ESlint
    - Überprüfung der Codequalität

- Containerisierung
  - Docker
    - Docker vs. Podman
  - Kubernetes

### Prof. Cochlovius

- Smart Home
  - Matter
    - Siehe Zahoransky
    - Cochlovius und Dörflinger

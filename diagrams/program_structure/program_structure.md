---
title: TTN Locator Program structure
---
<!-- https://mermaid.live -->
<!-- Use "garden" theme -->
```mermaid
flowchart TD
    subgraph TTNL [TTN Locator]
    TTNLF[TTN Locator Frontend]-->|makes API requests to|TTNLB[TTN Locator Backend]
    end
    TTNLB-->|makes API requests to|TTNM
    DVs[Devices]-->|send data to|GWs
    GWs[Gateways]-->|forward data to|TTN-LNS
    TTN-LNS[TTN LoRaWAN Network Server]-->|sends data with integration to|TTNM[TTN Mapper]
```
# HappyPets customer changes PTA using packet Delivery portal

## Customer access the web portal of Packet Delivery

The customer accesses the Packet Delivery Portal and the portal presents the customer the option to "Login with Credential". The portal presents a QR code.

```mermaid
sequenceDiagram
    participant HappyPetsAR
    participant HappyPetsIdP
    participant UniversalResolver
    participant CustomerSIOP
    actor Customer
    participant PacketDeliveryPortal
    participant PacketDeliveryProxy
    participant PacketDeliveryNode
    participant PacketDeliveryAR

    Customer->>+PacketDeliveryPortal: Accesses portal
    PacketDeliveryPortal->>-Customer: Select Login method
```

## Customer scans QR and initiates Authentication Request flow

```mermaid
sequenceDiagram
    participant HappyPetsAR
    participant HappyPetsIdP
    participant UniversalResolver
    participant CustomerSIOP
    actor Customer
    participant PacketDeliveryPortal
    participant PacketDeliveryProxy
    participant PacketDeliveryNode
    participant PacketDeliveryAR

    Customer->>+CustomerSIOP: Scan QR
    CustomerSIOP->>+PacketDeliveryProxy: POST /authentication-requests
```

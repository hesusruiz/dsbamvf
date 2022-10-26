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


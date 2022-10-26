```mermaid
sequenceDiagram
    participant HappyPetsAR;
    participant HappyPetsIdP;
    participant UniversalResolver;
    participant CustomerSIOP;
    actor Customer;
    participant PacketDeliveryPortal;
    participant PacketDeliveryProxy;
    participant PacketDeliveryNode;
    participant PacketDeliveryAR;

    actor->>+PacketDeliveryPortal: Accesses portal;
    PacketDeliveryPortal->>-actor: Select Login method;
```

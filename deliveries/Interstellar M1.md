# Milestone Delivery :mailbox:



**The [invoice form :pencil:](https://docs.google.com/forms/d/e/1FAIpQLSfmNYaoCgrxyhzgoKQ0ynQvnNRoTmgApz9NrMp-hd8mhIiO0A/viewform) has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](https://github.com/w3f/Grants-Program/blob/master/docs/milestone-deliverables-guidelines.md).**  

>The company registration is still pending and we did not yet received our VAT ID.
Invoice with "VAT ID pending" is compliant with french law. However, we will have to reissue the same invoice with the VAT ID as soon as we receive it. 

* **Application Document:** https://github.com/Interstellar-Network/Grants-Program/blob/Grant-application/applications/Interstellar-Network.md

**Context** (optional)

We refactored and changed the architecture of our pre-existing production grade Garbled Circuit Factory in order to integrate it with a substrate node. We take advantage  of this to split the architecture and separate the circuit generation from garbled circuit production.
 As a consequence, it took us more time than expected. Moreover, due to this architecture modification, we have adapted our deliverables accordingly:
 - we have now 2 Off Chain Workers with their respectives APIs, one for configuration and the logical circuit generation and one for thr garbled circuit production.
 - GCF substrate interface M1.1 will be managed with 2 gRPC servers with 2 apis that depend of circuit types.
 - M1.2 OCW CFG  handle configuration features,master files but also the generation of logical circuits.
 - M1.3 CLI is replaced by usage of substrate front end.
 - M1.4 OCW GCF manages Garbled Circuit production.

**Deliverables**


### Milestone 1 — Implement GCF Substrate modules


| Number | Deliverable | Link | Notes  |
| -----: | ----------- | -----------|------------ |
| 0b. | Documentation  |  [code documentation]( https://book.interstellar.gg/M1.html) |   |
| 0c. | Testing Guide | [testing guide](https://book.interstellar.gg/M1.html) | Core functions due to the specificity of the architecture are mainly covered with integration tests |
| 0d. | Docker | [docker api_garble](https://github.com/orgs/Interstellar-Network/packages/container/package/api_garble) `docker pull ghcr.io/interstellar-network/api_garble:milestone1` [docker api_circuit](https://github.com/orgs/Interstellar-Network/packages/container/package/api_circuits) `docker pull ghcr.io/interstellar-network/api_circuits:milestone1` |    |
| 0e. | Article | [article](https://book.interstellar.gg/M1.html)  |   will be published beginning of next week  |  
| 1. | GCF Substrate Interface  |[1: api_circuit](https://github.com/Interstellar-Network/api_circuits/tree/main) [2: api_garble](https://github.com/Interstellar-Network/api_garble)  |  GCF APIs is splitted |https://github.com/Interstellar-Network/api_garble/tree/w3f-milestone1 | We replaced GCF CFG with another GCF APIs for garbled circuit production  |  
| 2. | Substrate module: OCW GFG | [pallet ocwExample](https://github.com/Interstellar-Network/substrate-offchain-worker-demo/tree/interstellar/pallets/example-offchain-worker)| This OCW demo pallet i.e `ocwExample` manages the Master files for GCF configuration and the generation of logical circuits (used for production of garbled circuit managed by M1.4) 
| 3. | ~~Substrate GCF CFG CLI~~ |  | **CLI not needed anymore** Replaced by substrate front end and direct upload of config files/master files in IPFS | 
| 4. | Substrate module: OCW GCF | [pallet ocwDemo](https://github.com/Interstellar-Network/substrate-offchain-worker-demo/tree/interstellar/pallets/ocw)| This OCW demo pallet ie. `ocwDemo` manages the launch of Garbled Circuit production.
 

**Additional Information**
> Any further comments on the milestone that you would like to share with us.

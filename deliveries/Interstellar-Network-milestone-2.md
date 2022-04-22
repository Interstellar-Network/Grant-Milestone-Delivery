# Milestone Delivery :mailbox:



**The [invoice form :pencil:](https://docs.google.com/forms/d/e/1FAIpQLSfmNYaoCgrxyhzgoKQ0ynQvnNRoTmgApz9NrMp-hd8mhIiO0A/viewform) has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](https://github.com/w3f/Grants-Program/blob/master/docs/milestone-deliverables-guidelines.md).**  


* **Application Document:** https://github.com/w3f/Grants-Program/blob/master/applications/Interstellar-Network.md

* **Milestone Number:**  2

**Context** (optional)

This milestone focuses on the production of Display Garbled Circuit that will be used by the Trusted Transaction Validation Protocol TTVP. We show how those circuits are produced and how the result of their evaluation/execution are validated by the TTVP pallet. At this stage the TTVP pallet deliverable is still incomplete and implemented in OCW for demo purpose.
The next M3 milestone will focus on th execution of those circuits on the mobiles and on the TTVP friendly APIs that will hidden all the low-level complexity of circuit production and validation.


**Deliverables**


### Milestone 2 — GC Management in Substrate modules and Transaction Validation protocol use case (first part)


| Number | Deliverable | Link | Notes  |
| -----: | ----------- | -----------|------------ |
| 0a. | Licence  |  APACHE 2.0 & GPL3 | Only a part of the JustGarble repository is licenced with GPL3 and isolated with APIs | 
| 0b. | Documentation  |  [code documentation](https://book.interstellar.gg/M2.html) |   |
| 0c. | Testing Guide | [testing guide](https://book.interstellar.gg/M2.html#testing-guide) | Core functions due to the specificity of the architecture are mainly covered with integration tests |
| 0d. | Docker | [docker api_garble](https://github.com/orgs/Interstellar-Network/packages/container/package/api_garble) `docker pull ghcr.io/interstellar-network/api_garble:milestone1` [docker api_circuit](https://github.com/orgs/Interstellar-Network/packages/container/package/api_circuits) `docker pull ghcr.io/interstellar-network/api_circuits:milestone1` |  [How to use the dockers for demo:]( https://book.interstellar.gg/M2_demo_tutorial.html)     |
| 0e. | Article | [article](https://book.interstellar.gg/M2.html#article)  |   Will be published soon  |  
| 1. | Substrate Module: OCW GCF |   [OCW Circuits](https://github.com/Interstellar-Network/substrate-offchain-worker-demo/tree/interstellar-milestone2/pallets/ocw-circuits) and   [OCW Garble](https://github.com/Interstellar-Network/substrate-offchain-worker-demo/tree/interstellar-milestone2/pallets/ocw-garble)        | Manage the generation of Display Garbled Circuit to perform Transaction Validation |  
| 2. | Substrate module: pallet TTVP Transaction Validation Protocol | [pallet TTVP](https://github.com/Interstellar-Network/substrate-offchain-worker-demo/tree/interstellar-milestone2/pallets/tx-validation)    |  Pallet that will pilot the generation of Display Garbled Circuit to manage TTVP and the validation of their evaluation | 
| 3. | CLI Display Garbled Circuit Evaluation |  | Client to Evaluate Display Garbled Circuit to get One Time code used by TTVP | 

 

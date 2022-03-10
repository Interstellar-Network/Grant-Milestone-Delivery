# Milestone Delivery :mailbox:

> ⚡ Only the GitHub account that submitted the application is allowed to submit milestones. 
> 
> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with `>`, such as this one, can be removed.

**The [invoice form :pencil:](https://docs.google.com/forms/d/e/1FAIpQLSfmNYaoCgrxyhzgoKQ0ynQvnNRoTmgApz9NrMp-hd8mhIiO0A/viewform) has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](https://github.com/w3f/Grants-Program/blob/master/docs/milestone-deliverables-guidelines.md).**  

>The company registration is still pending and we did not yet get our VAT ID.
Invoice how mention a pending VAT ID is compliant with french law. However, we will have to reissue the same invoice with the VAT ID as soon as we receive it. 

* **Application Document:** https://github.com/Interstellar-Network/Grants-Program/blob/Grant-application/applications/Interstellar-Network.md

**Context** (optional)

We had to refactor/and change the architecture of our pre-existing production grade Garbled Circuit Factory in order to integrate it with a substrate node. We take advantage  of this to split the architecture and separate the circuit production from garbled circuit production.
 As a consequence, it took us more time than expected. Moreover, due to this architecture modification, we have adapted our deliverables accordingly:
 - only one OCW worker with 2 differents APIs, one for circuit production and one for garbled circuit production
 - GCF substrate interface M1.1 is replaced by GCF Circuit Interface Circuits and GCF substrate CFG M1.2 is replaced by GCF Interface GC in the deliverables.
 - OCW GCF M1.4 will manage both production and configuration. M1.3 not needed anymore.

**Deliverables**


### Milestone 1 — Implement GCF Substrate modules


| Number | Deliverable | Link | Notes  |
| -----: | ----------- | -----------|------------ |
| 0b. | Documentation  |  [code documentation]( https://book.interstellar.gg/M1.html) |   |
| 0c. | Testing Guide | [testing guide](https://book.interstellar.gg/M1.html) | Core functions due to the architecture are mainly covered with integration tests |
| 0d. | Docker | [docker file](https://book.interstellar.gg/M1.html) |    |
| 0e. | Article | [article](https://book.interstellar.gg/M1.html)  |   We will publish an **article**/workshop that explains what was done/achieved as part of the grant. (Content, language and medium should reflect your target audience described above.)  |  
| 1. | GCF Substrate Interface **Circuit** | https://github.com/Interstellar-Network/api_circuits  |  GCF APIs to manage circuits production. |  
| 2. |~~GCF CFG~~ GCF Substrate Interface **GC** | |   We replaced GCF CFG with another GCF APIs for garbled circuit production  |  
| 3. | ~~Substrate GCF CFG CLI~~ |  | **CLI not needed**. Configuration of OCW GCF will be managed later with substrate front end and/or governance module | 
| 4. | Substrate module: OCW GCF |  | This OCW pallet now  manage  both the launch of Circuit & Garbled Circuit production and the configuation features
 

**Additional Information**
> Any further comments on the milestone that you would like to share with us.

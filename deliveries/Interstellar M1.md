# Milestone Delivery :mailbox:

> ⚡ Only the GitHub account that submitted the application is allowed to submit milestones. 
> 
> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with `>`, such as this one, can be removed.

**The [invoice form :pencil:](https://docs.google.com/forms/d/e/1FAIpQLSfmNYaoCgrxyhzgoKQ0ynQvnNRoTmgApz9NrMp-hd8mhIiO0A/viewform) has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](https://github.com/w3f/Grants-Program/blob/master/docs/milestone-deliverables-guidelines.md).**  

* **Application Document:** Please, provide a link to the merged contract (the `.md` file in the [applications](https://github.com/w3f/Grants-Program/tree/master/applications) directory).
* **Milestone Number:** e.g. 1

**Context** (optional)
> Please provide a short paragraph or two connecting the deliverables in this milestone and describing their purpose.

**Deliverables**
> Please provide a list of all deliverables of the milestone extracted from the initial application and a link to the deliverable itself. Ideally all links inside the below table should include a commit hash, which will be used for testing. If you don't provide a commit hash, we will work off the default branch of your repository. Thus, if you plan on continuing work after delivery, we suggest you create a separate branch for either the delivery or your continuing work. 
> 
> If there is anything particular about any of the deliverables we or a future reader should know, use the respective `Notes` column.


### Milestone 1 — Implement GCF Substrate modules

- **Estimated duration:** 1 month
- **FTE:**  2.2
- **Costs:** 9,400 USD

| Number | Deliverable | Link | Notes  |
| -----: | ----------- | -----------|------------ |
| 0b. | Documentation  |  |     |
| 0c. | Testing Guide |  |  Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker |  |   We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article |   |   We will publish an **article**/workshop that explains what was done/achieved as part of the grant. (Content, language and medium should reflect your target audience described above.)  |  
| 1. | GCF Substrate Interface | |  GCF external service interface to interact with the following Substrate modules and IPFS. |  
| 2. | Substrate module: GCF CFG | |   We will create a Substrate GCF configuration pallet that will store GCF encrypted configuration information on chain (including cid of master circuit file, master key and other security parameter to ensure security of circuit production.  |  
| 3. | Substrate GCF CFG CLI|  | A CLI to set-up  GCF configuration pallet. | 
| 4. | Substrate module: OCW GCF |  | We will create an OCW pallet that will control and interact with GCF external service - Launch GC production and get resulted GC cid on IPFS. |  
 

**Additional Information**
> Any further comments on the milestone that you would like to share with us.

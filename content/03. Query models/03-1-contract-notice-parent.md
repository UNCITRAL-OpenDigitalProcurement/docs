## contractNoticeParent (cnParent) Query Model
---

|  **Attribute** | **Description** |  | **Usage** |  |
| :--- | :--- | :---: | :---: | :---: |
|   |  | **open** | **limited** | **selective** |
|  **ocid** | A globally unique identifier for this part of Contracting Process |  + | + | + |
|  **id** | An identifier for this particular release of information for part of CP | + | + | + |
|  **date** | The date this information was created/updated | + | + | + |
|  **tag** | A value from the [releaseTag codelist]() that identifies the nature of the release being made | + | + | + |
|  **initiationType** | String specifying the type of initiation process used for this part of CP, taken from the [initiationType codelist]() | + | + | + |
|  **planning.rationale** | The rationale for the procurement provided in free text. | + | + | + |
|  **planning.budget.description** | A short free text description of the budget source | + | + | + |
|  **planning.budget.amount** | Object described the sum of funds specified by CA this CP | + | + | + |
|  **planning.budget.isEuropeanUnionFunded** | True/False field to indicate whether this procurement is related to a project and/or programme financed by EU | + | + | + |
|  **planning.budget.budget Breakdown** | Detailed budget breakdown to be expressed, covering multiple budget sources and multiple periods. See [BudgetBreakdown]() | + | + | + |
|  **tender.id** | An identifier for this CP | + | + | + |
|  **tender.title** | Title for this CP | + | + | + |
|  **tender.description** | Description for this CP | + | + | + |
|  **tender.classification** | The primary classification for the tender. Uses CPV Codelist. See [Classification]() | + | + | + |
|  **tender.status** | The current status of the CP based on the [tenderStatus codelist]() | + | + | + |
|  **tender.statusDetails** | The current status of the CP based on the [tenderStatusDetails codelist]() | + | + | + |
|  **tender.value** | The total upper estimated value of this CP. See [Value]() | + | + | + |
|  **tender.procurementMethod** | Specify tendering method against the [procurementMethods codelist]() | + | + | + |
|  **tender.procurementMethodDetails** | Additional detail on the procurement method used. | + | + | + |
|  **tender.procurementMethodRationale** | Rationale of procurement method. | + | + | + |
|  **tender.procurementMethodAdditionalInfo** | Additional information about the procurement method. | + | + | + |
|  **tender.mainProcurementCategory** | The primary category describing the object of this contracting process from the [procurementCategory codelist]() | + | + | + |
|  **tender.additionalProcurementCategories** | Additional categories which describe the subject of this CP, from the [extendedProcurementCategory codelist]() | + | + | + |
|  **tender.hasEnquiries** | A true/false field to indicate whether any enquiries were received during the tender process | + | + | + |
|  **tender.eligibilityCriteria** | A description of any eligibility criteria for potential suppliers. | + | + | + |
|  **tender.submissionLanguages** | Language(s) in which tenderers may submit, drawn from the [submissionLanguages codelist]() | + | + | + |
|  **tender.contractPeriod** | The period over which the contract is estimated or required to be active. See [Period]() | + | + | + |
|  **tender.acceleratedProcedure.isAcceleratedProcedure** | A True/False field to indicate whether an accelerated procedure has been used for this procurement | + | + | + |
|  **tender.designContest.serviceContractAward** | A True/False field to indicate whether a service contract will be awarded to the winner(s) of the design contest. | + | + | + |
|  **tender.electronicWorkflows.useOrdering** | A True/False field to indicate if electronic ordering will be used. | + | + | + |
|  **tender.electronicWorkflows.usePayment** | A True/False field to indicate if electronic payment will be used. | + | + | + |
|  **tender.electronicWorkflows.acceptInvoicing** | A True/False field to indicate if electronic invoicing will be accepted. | + | + | + |
|  **tender.jointProcurement.isJointProcurement** | A True/False field to indicate if this is a joint procurement or not. | + | + | + |
|  **tender.procedureOutsourcing.procedureOutsourced** | A True/False field to indicate whether the procurement procedure has been outsourced | + | + | + |
|  **tender.framework.isAFramework** | A True/False field to indicate whether a framework agreement has been established as part of this procurement | + | + | + |
|  **tender.hasDynamicPurchasingSystem** | A True/False field to indicate whether a Dynamic Purchasing System has been set up. | + | + | + |
|  **tender.legalBasis** | The legal basis of the tender based on the [legalBasis codelist]() | + | + | + |
|  **tender.procuringEntity** | Link to the Organization operating this Process including a set of evaluation panel if declared by PE. See [OrganizationReference]() | + | + | + |
|  **relatedProcesses** | Objects described information about related funding (FSs), EI and other related sub-processes. See [RelatedProcess]() | + | + | + |
|  **parties** | Object described information about Entities involved into this CP. See [Organization]() | + | + | + |

 
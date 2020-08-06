## Query models

### contractNoticeParent (cnParent)
---

|  Attribute/description |  | Data-Type |
| --- | --- | --- |
|  **ocid** |  | string |
|  A globally unique identifier for this Contracting Process |  |  |
|  **id** |  | string |
|  An identifier for this particular release of information for CP |  |  |
|  **date** |  | date-time |
|  The date this information is released |  |  |
|  **tag** |  | string |
|  A value from the releaseTag codelist that identifies the nature of the release being made |  |  |
|  **initiationType** |  | string |
|  String specifying the type of initiation process used for this contract, taken from the initiationType codelist |  |  |
|  **planning.rationale** |  | string |
|  The rationale for the procurement provided in free text. |  |  |
|  **planning.budget.description** |  | string |
|  A short free text description of the budget source |  |  |
|  **planning.budget.amount** |  | object |
|  Object described the sum of funds specified by CA this CP <br/>See Value |  |  |
|  **planning.budget.isEuropeanUnionFunded** |  | boolean |
|  True/False field to indicate whether this procurement is related to a project and/or programme financed by EU |  |  |
|  **planning.budget.budget Breakdown** | array | object |
|  Detailed budget breakdown to be expressed, covering multiple budget sources and multiple periods<br/>See BudgetBreakdown |  |  |
|  **tender.id** |  | string |
|  An identifier for this CP |  |  |
|  **tender.title** |  | string |
|  Title for this CP |  |  |
|  **tender.description** |  | string |
|  Description for this CP |  |  |
|  **tender.classification** |  | object |
|  The primary classification for the tender. Uses CPV Codelist <br/>See Classification |  |  |
|  **tender.status** |  | string |
|  The current status of the CP based on the tenderStatus codelist |  |  |
|  **tender.statusDetails** |  | string |
|  The current status of the CP based on the tenderStatusDetails codelist |  |  |
|  **tender.value** |  | object |
|  The total upper estimated value of this CP<br/>See Value |  |  |
|  **tender.procurementMethod** |  | string |
|  Specify tendering method against the procurementMethods codelist |  |  |
|  **tender.procurementMethodDetails** |  | string |
|  Additional detail on the procurement method used. |  |  |
|  **tender.procurementMethodRationale** |  | string |
|  Rationale of procurement method |  |  |
|  **tender.procurementMethodAdditionalInfo** |  | string |
|  Additional information about the procurement method |  |  |
|  **tender.mainProcurementCategory** |  | string |
|  The primary category describing the object of this contracting process from the procurementCategory codelist |  |  |
|  **tender.additionalProcurementCategories** |  | string |
|  Additional categories which describe the subject of this CP, from the extendedProcurementCategory codelist |  |  |
|  **tender.hasEnquiries** |  | boolean |
|  A true/false field to indicate whether any enquiries were received during the tender process |  |  |
|  **tender.eligibilityCriteria** |  | string |
|  A description of any eligibility criteria for potential suppliers. |  |  |
|  **tender.submissionLanguages** | array | string |
|  Language(s) in which tenderers may submit, drawn from the submissionLanguages codelist |  |  |
|  **tender.contractPeriod** |  | object |
|  The period over which the contract is estimated or required to be active<br/>See Period |  |  |
|  **tender.acceleratedProcedure.isAcceleratedProcedure** |  | boolean |
|  A True/False field to indicate whether an accelerated procedure has been used for this procurement |  |  |
|  **tender.designContest.serviceContractAward** |  | boolean |
|  A True/False field to indicate whether a service contract will be awarded to the winner(s) of the design contest. |  |  |
|  **tender.electronicWorkflows.useOrdering** |  | boolean |
|  A True/False field to indicate if electronic ordering will be used. |  |  |
|  **tender.electronicWorkflows.usePayment** |  | boolean |
|  A True/False field to indicate if electronic payment will be used. |  |  |
|  **tender.electronicWorkflows.acceptInvoicing** |  | boolean |
|  A True/False field to indicate if electronic invoicing will be accepted. |  |  |
|  **tender.jointProcurement.isJointProcurement** |  | boolean |
|  A True/False field to indicate if this is a joint procurement or not. |  |  |
|  **tender.procedureOutsourcing.procedureOutsourced** |  | boolean |
|  A True/False field to indicate whether the procurement procedure has been outsourced |  |  |
|  **tender.framework.isAFramework** |  | boolean |
|  A True/False field to indicate whether a framework agreement has been established as part of this procurement |  |  |
|  **tender.hasDynamicPurchasingSystem** |  | boolean |
|  A True/False field to indicate whether a Dynamic Purchasing System has been set up. |  |  |
|  **tender.legalBasis** |  | string |
|  The legal basis of the tender based on the legalBasis codelist |  |  |
|  **tender.procuringEntity** |  | object |
|  Link to the Organization operating this Process including a set of evaluation panel if declared by PE <br/>See OrganizationReference |  |  |
|  **relatedProcesses** | array | object |
|  Objects described information about related funding (FSs), EI and other related sub-processes<br/>See RelatedProcess |  |  |
|  **parties** | array | object |
|  Object described information about Entities involved into this CP <br/>See Organization |  |  |


### contractNoticeDetails (cnDetails)
----
[
|  Attribute/description |  | Data-Type |
| --- | --- | --- |
|  **ocid** |  | string |
|  A globally unique identifier for this part of Contracting Process |  |  |
|  **id** |  | string |
|  An identifier for this particular release of information for part of CP |  |  |
|  **date** |  | date-time |
|  The date this information is released |  |  |
|  **tag** |  | string |
|  A value from the releaseTag codelist that identifies the nature of the release being made |  |  |
|  **initiationType** |  | string |
|  String specifying the type of initiation process used for this part of CP, taken from the initiationType codelist |  |  |
|  **purposeOfNotice.isACallForCompetition** |  | boolean |
|  A True/False field to indicate whether this notice is a call for competition |  |  |
|  **tender.id** |  | string |
|  An identifier for this part of CP |  |  |
|  **tender.title** |  | string |
|  Title for this part of CP |  |  |
|  **tender.description** |  | string |
|  Description for this part of CP |  |  |
|  **tender.awardCriteria** |  | string |
|  Specify the award criteria for the procurement, using the award criteria codelist |  |  |
|  **tender.status** |  | string |
|  The current status of this part of CP based on the tenderStatus codelist |  |  |
|  **tender.statusDetails** |  | string |
|  The current status of this part of CP based on the tenderStatusDetails codelist |  |  |
|  **tender.hasEnquiries** |  | boolean |
|  A true/false field to indicate whether any enquiries were received during the tender process. |  |  |
|  **tender.lotGroups.optionToCombine** |  | boolean |
|  True/False value indicates the CA reserves the right to combine the lots in this group when awarding a contract |  |  |
|  **tender.lots** | array | object |
|  A tender process is divided into lots. <br/>See Lot |  |  |
|  **tender.items** | array | object |
|  The goods and services to be purchased<br/>See Item |  |  |
|  **tender.requiresElectronicCatalogue** |  | boolean |
|  True/False value indicates whether bids must include an electronic catalogue. |  |  |
|  **tender.submissionMethod** |  | string |
|  Specify the method by which bids must be submitted using the submission method codelist |  |  |
|  **tender.submissionMethodRationale** |  | string |
|  A value from the submissionValueRationale codelist that identifies the rationale where electronic submission method is not to be allowed |  |  |
|  **tender.submissionMethodDetails** |  | string |
|  Any detailed or further information on the submission method. |  |  |
|  **tender.procurementMethodModalities** |  | string |
|  The modalities of the procurement method indicated with Method Modalities codelist |  |  |
|  **tender.documents** | array | object |
|  All documents and attachments related to the tender, including any notices. See the documentType codelist<br/>See Document |  |  |
|  **bids.statistics** | array | object |
|  Summary statistics on the number and nature of bids received. <br/>See BidStatistic |  |  |
|  **awards** | array | object |
|  A list of An award for the given procurement<br/>See Award |  |  |
|  **tender.awardPeriod** |  | object |
|  The period for adjudication and selection of the contract award<br/>See Period |  |  |
|  **contracts** | array | object |
|  Information regarding the signed contract between the buyer and supplier(s)<br/>See Contract |  |  |
|  **relatedProcesses** | array | object |
|  Objects described information about related funding (FSs), EI and other related sub-processes<br/>See RelatedProcess |  |  |
|  **parties** | array | object |
|  Object described information about Entities involved into this part of CP <br/>See Organization |  |  |
]($ "dddd")

### 
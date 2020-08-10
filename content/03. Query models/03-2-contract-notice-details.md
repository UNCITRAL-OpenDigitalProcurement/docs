## contractNoticeDetails (cnDetails) Query Model
---

|  **Attribute** | **Description** |  | **Usage** |  |
| :--- | :--- | :---: | :---: | :---: |
|   |  | **open** | **limited** | **selective** |
|  **ocid** | A globally unique identifier for this part of Contracting Process |  + | + | + |
|  **id** | An identifier for this particular release of information for part of CP | + | + | + |
|  **date** | The date this information was created/updated | + | + | + |
|  **tag** | A value from the [releaseTag codelist]() that identifies the nature of the release being made | + | + | + |
|  **initiationType** | String specifying the type of initiation process used for this part of CP, taken from the [initiationType codelist]() | + | + | + |
|  **purposeOfNotice.isACallForCompetition** | A True/False field to indicate whether this notice is a call for competition | + | + | + |
|  **tender.id** | An identifier for this part of CP | + | + | + |
|  **tender.title** | Title for this part of CP | + | + | + |
|  **tender.description** | Description for this part of CP | + | + | + |
|  **tender.awardCriteria** | Specify the award criteria for the procurement, using the [award criteria codelist]() | + | - | + |
|  **tender.awardCriteriaDetails** | Specify the award criteria details for the procurement, using the [award criteria details codelist]() | + | - | + |
|  **tender.conversions** | Conversions to be applied for the criteria. See [Conversion]() | + | - | + |
|  **tender.criteria** | Criteria required for the tenderers. See [Criterion]() | + | - | + |
|  **tender.status** | The current status of this part of CP based on the [tenderStatus codelist]() | + | + | + |
|  **tender.statusDetails** | The current status of this part of CP based on the [tenderStatusDetails codelist]() | + | + | + |
|  **tender.enquiryPeriod** | The period during which potential bidders may submit questions and requests for clarification. See [Period]() | + | - | + |
|  **tender.hasEnquiries** | A true/false field to indicate whether any enquiries were received during the tender process. | + | - | + |
|  **tender.enquiries** | List of received enquiries and comment from PE.See [Enquiry]() | + | - | + |
|  **tender.standStillPeriod** | The period for complaints. See [Period]() | + | + | + |
|  **tender.lotGroups.optionToCombine** | True/False value indicates the CA reserves the right to combine the lots in this group when awarding a contract | + | + | + |
|  **tender.lots** | A tender process is divided into lots. See [Lots]() | + | + | + |
|  **tender.items** | The goods and services to be purchased. See [Items](). | + | + | + |
|  **tender.requiresElectronicCatalogue** | True/False value indicates whether bids must include an electronic catalogue. | + | + | + |
|  **tender.submissionMethod** | Specify the method by which bids must be submitted using the [submission method codelist]() | + | + | + |
|  **tender.submissionMethodRationale** | A value from the [submissionValueRationale codelist]() that identifies the rationale where electronic submission method is not to be allowed | + | + | + |
|  **tender.submissionMethodDetails** | Any detailed or further information on the submission method. | + | - |  |
|  **tender.tenderPeriod** | The period when this part of CP will be open for submission. See [Period]() | + | - |  |
|  **tender.secondStage** | The number of participants in the second stage of GPA procedure. See [Period]() | - | - |  |
|  **tender.procurementMethodModalities** | The modalities of the procurement method indicated with [Method Modalities codelist]() | + | + |  |
|  **tender.otherCriteria** | The criteria. See [OtherCriteria]() | - | - |  |
|  **tender.auctionPeriod** | General period of all auctions scheduled under specific contracting process. See [Period]() | + | - |  |
|  **tender.electronicAuctions** | See [electronicAuctions]() | + |  |  |
|  **tender.documents** | All documents and attachments related to the tender, including any notices. See the [documentType codelist]() | + | + | + |
|  **tender.amendments** | An array of amendments for CP. See [Amendment]() | + | + | + |
|  **bids.details** | An array of bids, providing information on the bidders, bid status, bid values and related documents. See [Bids]() | + | - | + |
|  **bids.statistics** | Summary statistics on the number and nature of bids received. See [BidStatistic]() | + | - | + |
|  **awards** | A list of An award for the given procurement. See [Award]() | + | + | + |
|  **tender.awardPeriod** | The period for adjudication and selection of the contract award. See [Period]() | + | + |  |
|  **contracts** | Information regarding the signed contract between the buyer and supplier(s). See [Contract]() | + | + |  |
|  **relatedProcesses** | Objects described information about related funding (FSs), EI and other related sub-processes.See [RelatedProcess]() | + | + |  |
|  **parties** | Object described information about Entities involved into this part of CP. See [Organization]() | + | + |  |
|  **qualifications** | A list of an qualifications for the given procurement. See [Qualification]() | - | - |  |
|  **submissions.details** | An array of submissions, providing information on the candidates, status and related documents. See [Submission]() | - | - |  |
|  **preQualification.period** | The period when this part of CP will be open for submission. See [Period]() | - | - |  |
 
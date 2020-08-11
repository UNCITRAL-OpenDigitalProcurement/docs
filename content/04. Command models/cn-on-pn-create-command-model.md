## CNonPN Command model
---
|  **Code** | **Attribute** |  | **CNonPN** |  |  |
| :--- | :--- | :--- | :---: | --- | --- |
|   |  |  | open | limited | selective |
|   | **planning** |  | required | required | required |
|   | planning.rationale |  | optional | optional | optional |
|   | planning.budget |  | optional | optional | optional |
|   | planning.budget.description |  | optional | optional | optional |
|   | planning.budget.budgetBreakdown[] |  | inoperable | inoperable | inoperable |
|   | planning.budget.budgetBreakdown[].id |  | inoperable | inoperable | inoperable |
|   | planning.budget.budgetBreakdown[].amount.amount | has to be equal or less than budget.amount.amount in used FS | inoperable | inoperable | inoperable |
|   | planning.budget.budgetBreakdown[].amount.currency | The same value has to be delivered for each budgetBreakdown | inoperable | inoperable | inoperable |
|   | **tender** |  | required | required | required |
|   | tender.title |  | required | required | required |
|   | tender.description |  | required | required | required |
|   | tender.secondStage |  | inoperable | inoperable | optional |
|   | tender.secondStage.minimumCandidates |  | inoperable | inoperable | optional |
|   | tender.secondStage.maximumCandidates |  | inoperable | inoperable | optional |
|   | tender.otherCriteria |  | inoperable | inoperable | required |
|   | tender.otherCriteria.reductionCriteria |  | inoperable | inoperable | required |
|   | tender.otherCriteria.qualificationSystemMethods |  | inoperable | inoperable | required |
|   | tender.awardCriteria |  | required | required | required |
|   | tender.awardCriteriaDetails |  | required | inoperable | required |
|   | tender.procurementMethodAdditionalInfo |  | optional | optional | optional |
|   | tender.procuringEntity |  | optional | optional | optional |
|   | tender.procuringEntity.id |  | required | required | required |
|   | tender.procuringEntity.persones |  | optional | optional | optional |
|   | tender.procuringEntity.persones.title |  | required | required | required |
|   | tender.procuringEntity.persones.name |  | required | required | required |
|   | tender.procuringEntity.persones.identifier |  | required | required | required |
|   | tender.procuringEntity.persones.identifier.id |  | required | required | required |
|   | tender.procuringEntity.persones.iidentifier.scheme |  | required | required | required |
|   | tender.procuringEntity.persones.identifier.uri |  | optional | optional | optional |
|   | tender.procuringEntity.persones.businessFunctions |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.type |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.id |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.jobTitle |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.period |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.period.startDate |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.documents |  | optional | optional | optional |
|   | tender.procuringEntity.persones.businessFunctions.documents.description |  | optional | optional | optional |
|   | tender.procuringEntity.persones.businessFunctions.documents.title |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.documents.id |  | required | required | required |
|   | tender.procuringEntity.persones.businessFunctions.documents.documentType |  | required | required | required |
|   | tender.criteria |  | optional | inoperable | optional |
|   | tender.criteria[].id | At least 1 entry | required | inoperable | required |
|   | tender.criteria[].title |  | required | inoperable | required |
|   | tender.criteria[*].description |  | optional | inoperable | optional |
|   | tender.criteria[*].source |  | optional | inoperable | optional |
|   | tender.criteria[*].classification.scheme |  | optional | inoperable | optional |
|   | tender.criteria[*].classification.id |  | optional | inoperable | optional |
|   | tender.criteria[*].classification.description |  | optional | inoperable | optional |
|   | tender.criteria[*].relatesTo |  | optional | inoperable | optional |
|   | tender.criteria[*].relatedItem |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*] |  | required | inoperable | required |
|   | tender.criteria[*].requirementGroups[*].id | At least 1 entry | required | inoperable | required |
|   | tender.criteria[*].requirementGroups[*].description |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*].requirements[*] |  | required |  | required |
|   | tender.criteria[*].requirementGroups[*].requirements[*].id | At least 1 entry | required | inoperable | required |
|   | tender.criteria[*].requirementGroups[*].requirements[*].title |  | required | inoperable | required |
|   | tender.criteria[*].requirementGroups[*].requirements[*].description |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*].requirements[*].dataType |  | required | inoperable | required |
|   | tender.criteria[*].requirementGroups[*].requirements[*].exepctedValue |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*].requirements[*].minValue |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*].requirements[*].maxValue |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.startDate |  | required | inoperable | required |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.endDate |  | required | inoperable | required |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.durationInMonth |  | optional | inoperable | optional |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.duration |  | optional | inoperable | optional |
|   | tender.conversions[*] | At least 1 entry | optional | inoperable | optional |
|   | tender.conversions[*].id |  | required | inoperable | required |
|   | tender.conversions[*].relatesTo |  | optional | inoperable | optional |
|   | tender.conversions[*].relatedItem |  | required | inoperable | required |
|   | tender.conversions[*].description |  | optional | inoperable | optional |
|   | tender.conversions[*].rationale |  | required | inoperable | required |
|   | tender.conversions[*].coefficients[*] | At least 1 entry | required | inoperable | required |
|   | tender.conversions[*].coefficients[*].id |  | required | inoperable | required |
|   | tender.conversions[*].coefficients[*].value |  | required | inoperable | required |
|   | tender.conversions[*].coefficients[*].coefficients |  | required | inoperable | required |
|   | tender.conversions[*].coefficients[*].minValue |  | optional | inoperable | optional |
|   | tender.conversions[*].coefficients[*].maxValue |  | optional | inoperable | optional |
|   | tender.conversions[*].coefficients[*].period.startDate |  | optional | inoperable | optional |
|   | tender.conversions[*].coefficients[*].period.endDate |  | optional | inoperable | optional |
|   | tender.conversions[*].coefficients[*].period.durationInMonth |  | optional | inoperable | optional |
|   | tender.conversions[*].coefficients[*].period.duration |  | optional | inoperable | optional |
|   | tender.tenderPeriod |  | required | inoperable | inoperable |
|   | tender.tenderPeriod.endDate |  | required | inoperable | inoperable |
|   | tender.enquiryPeriod |  | required | inoperable | inoperable |
|   | tender.enquiryPeriod.endDate |  | required | inoperable | inoperable |
|   | tender.documents[*] |  | required | required | required |
|   | tender.documents[*].id |  | required | required | required |
|   | tender.documents[*].documentType |  | required | required | required |
|   | tender.documents[*].title |  | required | required | required |
|   | tender.documents[*].description |  | optional | optional | optional |
|   | tender.documents[*].relatedLots[*] | At least 1 entry | optional | optional | optional |
|   | tender.procurementMethodRationale |  | optional | optional | optional |
|   | tender.procurementMethodModalities |  | optional | inoperable | optional |
|   | tender.electronicAuctions |  | optional | inoperable | optional |
|   | tender.electronicAuctions.details.id | At least 1 entry | required | inoperable | required |
|   | tender.electronicAuctions.details.relatedLot |  | required | inoperable | required |
|   | tender.electronicAuctions.details.electronicAuctionModalities |  | required | inoperable | required |
|   | tender.electronicAuctions.details.electronicAuctionModalities[*].eligibleMinimumDifference |  | required | inoperable | required |
|   | tender.electronicAuctions.details.electronicAuctionModalities[*].eligibleMinimumDifference.amount |  | required | inoperable | required |
|   | tender.electronicAuctions.details.electronicAuctionModalities[*].eligibleMinimumDifference.currency |  | required | inoperable | required |
|   | tender.lots[*] |  | required | required | required |
|   | tender.lots[*].id | Lots object have to include at least one lot | required | required | required |
|   | tender.lots[*].title |  | required | required | required |
|   | tender.lots[*].description |  | required | required | required |
|   | tender.lots[*].internalId |  | optional | optional | optional |
|   | tender.lots[*].value |  | required | required | required |
|   | tender.lots[*].value.amount | the cumulative sum of all added tender.lot.value.amount has to be equal or less than the sum of all added budget.budgetBreakdown.amount.amount | required | required | required |
|   | tender.lots[*].value.currency | *tender.lot.value.currency in all added lots has to be equal to budget.budgetBreakdown.amount.currency* | required | required | required |
|   | tender.lots[*].contractPeriod |  | required | required | required |
|   | tender.lots[*].contractPeriod.startDate | - tender.lot.contractPeriod.startDate has to be earlier than Tender.lot.contractPeriod.endDate in one lot object & tender.lot.contractPeriod.startDate has to be later than tender.tenderPeriod.endDate<br/>- earliest value among all added tender.lot.contractPeriod.startDate has to be earlier than values of all added planning.budget.budgetBreakdown.period.endDate | required | required | required |
|   | tender.lots[*].contractPeriod.endDate | - the latest value among all added tender.lot.contractPeriod.endDate has to be later than values of all added planning.budget.budgetBreakdown.period.startDate | required | required | required |
|   | tender.lots[*].placeOfPerformance |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.description |  | optional | optional | optional |
|   | tender.lots[*].placeOfPerformance.address |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.streetAddress |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.locality |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.locality.id |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.locality.description |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.locality.scheme |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.region |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.region.id |  | required | required | required |
|   | tender.llots[*].placeOfPerformance.address.postalCode |  | optional | optional | optional |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.country |  | required | required | required |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.country.id |  | required | required | required |
|   | tender.items |  | required | required | required |
|   | tender.items[*].id | At least 1 entry | required | required | required |
|   | tender.items[*].description |  | required | required | required |
|   | tender.items[].internalId |  | optional | optional | optional |
|   | tender.items[].classification |  | required | required | required |
|   | tender.items[].classification.id |  | required | required | required |
|   | tender.items[].addtionalClassification |  | optional | optional | optional |
|   | tender.items[].addtionalClassification.id |  | required | required | required |
|   | tender.items[].quantity |  | required | required | required |
|   | tender.items[].unit |  | required | required | required |
|   | tender.items[].unit.id |  | required | required | required |
|   | tender.items[].relatedLot |  | required | required | required |
|   | **preQualification** |  |  |  |  |
|   | preQualification.period |  | inoperable | inoperable | required |
|   | preQualification.period.endDate |  | inoperable | inoperable | required |
## CNonPN Command model

|   | **Attribute** |  | **PN** |  | **CNonPN** |  |  |
| :--- | :--- | :--- | :---: | --- | :---: | --- | --- |
|   |  |  | **pn** | **pin** | **open** | **limited** | **selective** |
|   | **planning** |  | required | required | required | required | required |
|   | planning.rationale |  | optional | optional | optional | optional | optional |
|   | planning.budget.description |  | optional | optional | optional | optional | optional |
|   | planning.budget.budgetBreakdown[].id |  | required | required | inoperable | inoperable | inoperable |
|   | planning.budget.budgetBreakdown[].amount.amount | has to be equal or less than budget.amount.amount in used FS | required | required | inoperable | inoperable | inoperable |
|   | planning.budget.budgetBreakdown[].amount.currency | The same value has to be delivered for each budgetBreakdown | required | required | required | required | required |
|   | **tender** |  | required | required | required | required | required |
|   | tender.title |  | required | required | required | required | required |
|   | tender.description |  | required | required | required | required | required |
|   | tender.secondStage.minimumCandidates |  | inoperable | inoperable | inoperable | inoperable | optional |
|   | tender.secondStage.maximumCandidates |  | inoperable | inoperable | inoperable | inoperable | optional |
|   | tender.otherCriteria |  | inoperable | inoperable | inoperable | inoperable | required |
|   | tender.otherCriteria.reductionCriteria |  | inoperable | inoperable  | inoperable | inoperable | required |
|   | tender.otherCriteria.qualificationSystemMethods |  | inoperable | inoperable | inoperable | inoperable | required |
|   | tender.awardCriteria |  | inoperable | inoperable | required | required | required |
|   | tender.awardCriteriaDetails |  | inoperable | inoperable | required | required | required |
|   | tender.procurementMethodAdditionalInfo |  | inoperable | inoperable | optional | optional | optional |
|   | tender.legalBasis |  | required | required | required | required | required |
|   | tender.submissionLanguages[*] |  | optional | optional | optional | optional | optional |
|   | tender.procuringEntity |  |  |  |  |  |  |
|   | tender.procuringEntity.name |  |  |  |  |  |  |
|   | tender.procuringEntity.identifier.scheme |  |  |  |  |  |  |
|   | tender.procuringEntity.identifier.id |  |  |  |  |  |  |
|   | tender.procuringEntity.identifier.legalName |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalIdentifiers[*].scheme |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalIdentifiers[*].id |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalIdentifiers[*].legalName |  |  |  |  |  |  |
|   | tender.procuringEntity.contactPoint.id |  |  |  |  |  |  |
|   | tender.procuringEntity.contactPoint.name |  |  |  |  |  |  |
|   | tender.procuringEntity.contactPoint.email |  |  |  |  |  |  |
|   | tender.procuringEntity.contactPoint.telephone |  |  |  |  |  |  |
|   | tender.procuringEntity.contactPoint.url |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalContactPoints[*].id |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalContactPoints[*].name |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalContactPoints[*].email |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalContactPoints[*].telephone |  |  |  |  |  |  |
|   | tender.procuringEntity.additionalContactPoints[*].url |  |  |  |  |  |  |
|   | tender.procuringEntity.address.streetAddress |  |  |  |  |  |  |
|   | tender.procuringEntity.address.locality |  |  |  |  |  |  |
|   | tender.procuringEntity.address.region |  |  |  |  |  |  |
|   | tender.procuringEntity.address.postalCode |  |  |  |  |  |  |
|   | tender.procuringEntity.address.countryName |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.countryDetails.schema |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.countryDetails.id |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.countryDetails.description |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.regionDetails.schema |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.regionDetails.id |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.regionDetails.description |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.localityDetails.schema |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.localityDetails.id |  |  |  |  |  |  |
|   | tender.procuringEntity.address.addressDetails.localityDetails.description |  |  |  |  |  |  |
|   | tender.procuringEntity.details.typeOfBuyer |  |  |  |  |  |  |
|   | tender.procuringEntity.details.classifications[*].scheme |  |  |  |  |  |  |
|   | tender.procuringEntity.details.classifications[*].id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.classifications[*].description |  |  |  |  |  |  |
|   | tender.procuringEntity.details.mainGeneralActivity |  |  |  |  |  |  |
|   | tender.procuringEntity.details.mainSectoralActivity |  |  |  |  |  |  |
|   | tender.procuringEntity.details.legalForm[*].scheme |  |  |  |  |  |  |
|   | tender.procuringEntity.details.legalForm[*].id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.legalForm[*].description |  |  |  |  |  |  |
|   | tender.procuringEntity.details.isACentralPurchasingBody |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].bankName |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].identifier.scheme |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].identifier.id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].identifier.legalName |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].accountIdentification.scheme |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].accountIdentification.id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].accountIdentification.legalName |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.streetAddress |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.locality |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.region |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.postalCode |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.countryName |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.countryDetails.schema |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.countryDetails.id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.countryDetails.description |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.regionDetails.schema |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.regionDetails.id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.regionDetails.description |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.localityDetails.schema |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.localityDetails.id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].address.addressDetails.localityDetails.description |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].additionalAccountIndentifiers[*].scheme |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].additionalAccountIndentifiers[*].id |  |  |  |  |  |  |
|   | tender.procuringEntity.details.bankAccounts[*].additionalAccountIndentifiers[*].description |  |  |  |  |  |  |
|   | tender.criteria[*].id | At least 1 entry |  |  |  |  |  |
|   | tender.criteria[*].title |  | inoperable | optional | optional | optional | optional |
|   | tender.criteria[*].description |  |  |  |  |  |  |
|   | tender.criteria[*].source |  |  |  |  |  |  |
|   | tender.criteria[*].classification.scheme |  |  |  |  |  |  |
|   | tender.criteria[*].classification.id |  |  |  |  |  |  |
|   | tender.criteria[*].classification.description |  |  |  |  |  |  |
|   | tender.criteria[*].relatesTo |  |  |  |  |  |  |
|   | tender.criteria[*].relatedItem |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].id | At least 1 entry |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].description |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].id | At least 1 entry |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].title |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].description |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].dataType |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].exepctedValue |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].minValue |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].maxValue |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.startDate |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.endDate |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.durationInMonth |  |  |  |  |  |  |
|   | tender.criteria[*].requirementGroups[*].requirements[*].period.duration |  |  |  |  |  |  |
|   | tender.conversions[*].id | At least 1 entry | inoperable | optional | optional | optional | optional |
|   | tender.conversions[*].relatesTo |  |  |  |  |  |  |
|   | tender.conversions[*].relatedItem |  |  |  |  |  |  |
|   | tender.conversions[*].description |  |  |  |  |  |  |
|   | tender.conversions[*].rationale |  |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].id | At least 1 entry |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].value |  |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].minValue |  |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].maxValue |  |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].period.startDate |  |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].period.endDate |  |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].period.durationInMonth |  |  |  |  |  |  |
|   | tender.conversions[*].coefficients[*].period.duration |  |  |  |  |  |  |
|   | tender.tenderPeriod.startDate |  | required | required | inoperable | inoperable | inoperable |
|   | tender.tenderPeriod.endDate |  | inoperable | inoperable | required | required | inoperable |
|   | tender.documents[*].id | The values of tender.documents.relatedLots of all delivered documents to be matched with all delivered tender.lots.id | optional | optional | optional | optional | optional |
|   | tender.documents[*].name |  |  |  |  |  |  |
|   | tender.documents[*].documentType |  |  |  |  |  |  |
|   | tender.documents[*].title |  |  |  |  |  |  |
|   | tender.documents[*].description |  |  |  |  |  |  |
|   | tender.documents[*].uri |  |  |  |  |  |  |
|   | tender.documents[*].relatedLots[*] | At least 1 entry |  |  |  |  |  |
|   | tender.procurementMethodRationale |  | optional | optional | optional | optional | optional |
|   | tender.procurementMethodModalities |  | optional | optional | optional | optional | optional |
|   | tender.electronicAuctions.details.id | At least 1 entry | inoperable | inoperable | optional | inoperable | optional |
|   | tender.electronicAuctions.details.relatedLot |  |  |  |  |  |  |
|   | tender.electronicAuctions.details.electronicAuctionModalities[*].eligibleMinimumDifference.value.amount |  |  |  |  |  |  |
|   | tender.electronicAuctions.details.electronicAuctionModalities[*].eligibleMinimumDifference.value.currency |  |  |  |  |  |  |
|   | tender.electronicAuctions.details.electronicAuctionModalities[*].uri |  |  |  |  |  |  |
|   | tender.lots[*].id | Lots object have to include at least one lot |  |  |  |  |  |
|   | tender.lots[*].title |  |  |  |  |  |  |
|   | tender.lots[*].description |  |  |  |  |  |  |
|   | tender.lots[*].internalId |  |  |  |  |  |  |
|   | tender.lots[*].value.amount | the cumulative sum of all added tender.lot.value.amount has to be equal or less than the sum of all added budget.budgetBreakdown.amount.amount |  |  |  |  |  |
|   | tender.lots[*].value.currency | *tender.lot.value.currency in all added lots has to be equal to budget.budgetBreakdown.amount.currency* |  |  |  |  |  |
|   | tender.lots[*].contractPeriod.startDate | - tender.lot.contractPeriod.startDate has to be earlier than Tender.lot.contractPeriod.endDate in one lot object & tender.lot.contractPeriod.startDate has to be later than tender.tenderPeriod.endDate<br/>- earliest value among all added tender.lot.contractPeriod.startDate has to be earlier than values of all added planning.budget.budgetBreakdown.period.endDate |  |  |  |  |  |
|   | tender.lots[*].contractPeriod.endDate | - the latest value among all added tender.lot.contractPeriod.endDate has to be later than values of all added planning.budget.budgetBreakdown.period.startDate |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.description |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.streetAddress |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.locality |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.region |  |  |  |  |  |  |
|   | tender.llots[*].placeOfPerformance.address.postalCode |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.countryName |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.countryDetails.schema |  |  |  |  |  |  |
|   | tender.llots[*].placeOfPerformance.address.addressDetails.countryDetails.id |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.countryDetails.description |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.regionDetails.schema |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.regionDetails.id |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.regionDetails.description |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.localityDetails.schema |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.localityDetails.id |  |  |  |  |  |  |
|   | tender.lots[*].placeOfPerformance.address.addressDetails.localityDetails.description |  |  |  |  |  |  |
|   | tender.items[*].id | At least 1 entry |  |  |  |  |  |
|   | tender.items[*].description |  |  |  |  |  |  |
|   | tender.items[*].classification.scheme | same as tender/lot? |  |  |  |  |  |
|   | tender.items[*].classification.id | - All added tender.Item.classification.id in all items coincide by first 3 figures in codes<br/>- All added tender.Item.classification.id in all items coincide by first 3 figures of value of tender.classification.id in EI |  |  |  |  |  |
|   | tender.items[*].classification.description |  |  |  |  |  |  |
|   | tender.items[*].relatedLots[*] | Values of tender.items.relatedLot for all Items have to be matched with all delivered lots by tender.lots.id |  |  |  |  |  |
|   | tender.items[*].quantity |  |  |  |  |  |  |
|   | tender.items[*].additionalClassifications[*].scheme |  |  |  |  |  |  |
|   | tender.items[*].additionalClassifications[*].id |  |  |  |  |  |  |
|   | tender.items[*].additionalClassifications[*].description |  |  |  |  |  |  |
|   | tender.items[*].internalId |  |  |  |  |  |  |
|   | tender.items[*].unit.scheme |  |  |  |  |  |  |
|   | tender.items[*].unit.id |  |  |  |  |  |  |
|   | tender.items[*].unit.name |  |  |  |  |  |  |
|   | **preQualification** |  |  |  |  |  |  |
|   | preQualification.period.endDate |  |  |  |  |  |  |
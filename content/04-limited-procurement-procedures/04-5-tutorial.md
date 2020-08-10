## Tutorial
___

### Create PN

Before creating a CP, follow these steps:

* Create [EI]() and [FS]().
* Get [X-OPERATION-ID]().
* Register [documents]()

**Send request**


* POST /do/pn?country=MD&pmd=... HTTP/1.1
* Authorization: Bearer QWxhZGRpbjpPcGVuU2VzYW1l
* X-OPERATION-ID: Got in preconditions steps
* Content-Type: application/json
* Host: bpe.eprocurement.systems


|List of supported pmd`s: |  |
| --   |     ---             |
| DA   | Direct Award        |
| NP   | Negotiation Process |
| OP   | Other Procedure     |


Use the JSON schema below and [command model]() to create the payload:

```json
{
	"planning": {
		"rationale": "string",
		"budget": {
			"description": "string",
			"budgetBreakdown": [{
				"id": "fs-id-uuid",
				"amount": {
					"amount": 100,
					"currency": "MDL"
				}
			}]
		}
	},
	"tender": {
		"title": "string",
		"procurementMethodRationale": "string",
		"procurementMethodAdditionalInfo": "string ",
		"description": "string",
		"legalBasis": "string",
		"tenderPeriod": {
			"startDate": "2019-11-01T00:00:00Z"
		},
		"lots": [{
			"id": "string",
			"title": "string",
			"description": "string",
			"value": {
				"amount": 100,
				"currency": "MDL"
			},
			"contractPeriod": {
				"startDate": "2020-08-25T00:00:00Z",
				"endDate": "2020-08-30T00:00:00Z"
			},
			"placeOfPerformance": {
				"address": {
					"streetAddress": "string",
					"postalCode": "string",
					"addressDetails": {
						"country": {
							"id": "string"
						},
						"region": {
							"id": "string"
						},
						"locality": {
							"scheme": "string",
							"id": "string",
							"description": "string"
						}
					}
				}
			}
		}],
		"items": [{
			"id": "string",
			"classification": {
				"scheme": "string",
				"description": "string",
				"id": "string"

			},
			"additionalClassifications": [{
				"scheme": "string",
				"description": "string",
				"id": "string"
			}],
			"quantity": 100,
			"unit": {
				"id": "string",
				"name": "string"
			},
			"description": "string",
			"relatedLot": "string"
		}],
		"documents": [{
			"documentType": "string",
			"title": "string",
			"description": "string",
			"id": "85e69404-d32c-4235-ba2c-e9a7672fbd7a-1573637801126",
			"relatedLots": [
				"string"
			]
		}],
		"procuringEntity": {
			"name": "string",
			"identifier": {
				"scheme": "string",
				"id": "string",
				"legalName": "string",
				"uri": "string"
			},
			"contactPoint": {
				"name": "string",
				"email": "string",
				"telephone": "string",
				"faxNumber": "string",
				"url": "string"
			},
			"additionalIdentifiers": [{
				"scheme": "string",
				"id": "string",
				"legalName": "string"
			}],
			"address": {
				"streetAddress": "string",
				"postalCode": "string",
				"addressDetails": {
					"country": {
						"id": "string"
					},
					"region": {
						"id": "string"
					},
					"locality": {
						"scheme": "string",
						"id": "string",
						"description": "string"
					}
				}
			}
		}
	}
}

```

### Update PN
---

**Send request**


* POST /do/pn/cpid/ocid-pn HTTP/1.1
* Authorization: Bearer QWxhZGRpbjpPcGVuU2VzYW1l
* X-OPERATION-ID: Got in preconditions steps
* Content-Type: application/json
* Host: bpe.eprocurement.systems


Use the JSON schema below and [command model]() to create the payload:


```json
{
	"planning": {
		"rationale": "string",
		"budget": {
			"description": "string",
			"budgetBreakdown": [{
				"id": "fs-id-uuid",
				"amount": {
					"amount": 100,
					"currency": "MDL"
				}
			}]
		}
	},
	"tender": {
		"title": "string",
		"procurementMethodRationale": "string",
		"procurementMethodAdditionalInfo": "string ",
		"description": "string",
		"legalBasis": "string",
		"tenderPeriod": {
			"startDate": "2019-11-01T00:00:00Z"
		},
		"lots": [{
			"id": "string",
			"title": "string",
			"description": "string",
			"value": {
				"amount": 100,
				"currency": "MDL"
			},
			"contractPeriod": {
				"startDate": "2020-08-25T00:00:00Z",
				"endDate": "2020-08-30T00:00:00Z"
			},
			"placeOfPerformance": {
				"address": {
					"streetAddress": "string",
					"postalCode": "string",
					"addressDetails": {
						"country": {
							"id": "string"
						},
						"region": {
							"id": "string"
						},
						"locality": {
							"scheme": "string",
							"id": "string",
							"description": "string"
						}
					}
				}
			}
		}],
		"items": [{
			"id": "string",
			"classification": {
				"scheme": "string",
				"description": "string",
				"id": "string"

			},
			"additionalClassifications": [{
				"scheme": "string",
				"description": "string",
				"id": "string"
			}],
			"quantity": 100,
			"unit": {
				"id": "string",
				"name": "string"
			},
			"description": "string",
			"relatedLot": "string"
		}],
		"documents": [{
			"documentType": "string",
			"title": "string",
			"description": "string",
			"id": "85e69404-d32c-4235-ba2c-e9a7672fbd7a-1573637801126",
			"relatedLots": [
				"string"
			]
		}],
		"procuringEntity": {
			"name": "string",
			"identifier": {
				"scheme": "string",
				"id": "string",
				"legalName": "string",
				"uri": "string"
			},
			"contactPoint": {
				"name": "string",
				"email": "string",
				"telephone": "string",
				"faxNumber": "string",
				"url": "string"
			},
			"additionalIdentifiers": [{
				"scheme": "string",
				"id": "string",
				"legalName": "string"
			}],
			"address": {
				"streetAddress": "string",
				"postalCode": "string",
				"addressDetails": {
					"country": {
						"id": "string"
					},
					"region": {
						"id": "string"
					},
					"locality": {
						"scheme": "string",
						"id": "string",
						"description": "string"
					}
				}
			}
		}
	}
}

```

**Result:**

* Synchronous response from server: **202 Accepted**
* Feed Point Response: 

``` json

{
  "initiator": "platform",
  "X-OPERATION-ID": "f5c6a3c0-5ff8-463f-9c0c-d4c1f324b7fb",
  "X-RESPONSE-ID": "f5c6a3c1-5ff8-463f-9c0c-d4c1f324b7fb",
  "data": {
    "ocid": "ocds-000-00001",
    "url": "http://public.eprocurement.systems/tenders/ocds-000-00001/ocds-000-00001-pn",
    "operationDate": "2018-08-14T13:51:06Z"
  }
}

```

## Create CNonPN
---

* POST /do/pn/cpid/ocid-pn HTTP/1.1
* Authorization: Bearer QWxhZGRpbjpPcGVuU2VzYW1l
* X-OPERATION-ID: Got in preconditions steps
* Content-Type: application/json
* Host: bpe.eprocurement.systems

```json


```
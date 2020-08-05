# Limited procurement procedures
## Table of contents
___

  1. [Introduction](#introduction)
  2. [Quickstart]()
  3. [Command model]()
  4. [Query model]()

## Introduction
___
CA is able to maintain the registration of information regarding single source procedures carried out of the eProcurement system and the execution of the process inside the system as well. Having entered the information regarding the procedure, CA enters information on the winner and the agreement. 
The procurement process is carried out in the following sequence:

<img src="https://raw.githubusercontent.com/UNCITRAL-OpenDigitalProcurement/docs/master/images/1.png" width="80%" height="80%" />

### Publication of a decision on intent to conclude an agreement
CA publishes the concluded agreement and enters information regarding the EO immediately. This information is published as a report on the concluded agreement. It is not possible to submit a complaint at this point.

### Entering information on EO on the basis of the concluded agreement
CA enters information on EO on the basis of the concluded agreement. Editing is possible only until the report activation made by CA. Additionally CA notes compliance with qualification criteria for a certain EO on the agreement. Once the EO is determined, no further actions are performed by the CA.

### Concluding an agreement
Once the EO information is entered, CA can publish the concluded agreement. Conclusion of agreement, report on the introduced changes into the agreement, and execution of agreement are executed in the following way:
  * Changes of the agreement’s status to active or terminated, should be certified with EDS as a matter of course.
  * Entering information on the agreement is optional. Upon affixation of EDS, CA can finish the procedure (complete).
 
### Procedure completion
Once the agreement was uploaded and EDS added, the procedure automatically changes to ‘complete’ status.

## Quickstart
___
### Preconditions

Before creating a CP, follow these steps:

* Create [EI]() and [FS]().
* Get [X-OPERATION-ID]().
* Register [documents]()

### Create PN

**Send request**


* POST /do/pn?country=...&pmd=... HTTP/1.1
* Authorization: Bearer QWxhZGRpbjpPcGVuU2VzYW1l
* X-OPERATION-ID: Got in preconditions steps
* Content-Type: application/json
* Host: bpe.eprocurement.systems


|List of supported pmd`s: |  |
| --   |     ---             |
| DA   | Direct Award        |
| NP   | Negotiation Process |
| OP   | Other Procedure     |


Use the JSON schema below to create the payload:

[](/schema/limited_pn_create.schema.json)

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
    "operationDate": "2018-08-14T13:51:06Z",
    "outcomes": {
      "pn": [
        {
          "id": "ocds-t1s2t3-TEST-PN",
          "X-TOKEN": "c3bdd497-ac2d-4e25-bd7f-cd55111aa7b4"
        }
      ]
    }
  }
}

```

### Update PN

**Send request**


* POST /do/pn/cpid/ocid-pn HTTP/1.1
* Authorization: Bearer QWxhZGRpbjpPcGVuU2VzYW1l
* X-OPERATION-ID: Got in preconditions steps
* Content-Type: application/json
* Host: bpe.eprocurement.systems

Use the JSON schema below to create the payload:

Use the JSON schema below to create the payload:

[](/schema/limited_pn_create.schema.json)

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

## Command model
___
## Query model
___


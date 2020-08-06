## Query model
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


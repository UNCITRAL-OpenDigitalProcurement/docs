## Transport model
----

CN described as Record Package consists of four (at least) or more Release Packages: 
* ‘cnParent’ (hi-level common data of Contract Notice and a budget of procurement)
* ‘cnDetails’ with all other CN data (depends on the starting point (stage): PN, PIN or CfC (PS/PQ/EV)
* ‘eiDetails’ (hi-level common data of used EI)
* At least one ‘fs’ (detailed information about used FS)  

```json

{
  "uri": "",
  "version": "",
  "extensions": [],
  "publisher": {},
  "license": "",
  "publishedDate": "",
  "packages": [
    "uri of EI release package",
    "uri(s) of FS(s) release package(s)",
    "uri of CN hi-level release package",
    "uri of CN details release package"
  ],
  "records": [
    {
      "description": "This Compiled release includes CN's hi-level",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/cnParent"}
      }
    },
    {
      "description": "This compiled release includes CN's details",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/cnDetails"}
      }
    },
    {
      "description": "This compiled release includes FS details",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/fs"}
      }
    },
    {
      "description": "This Compiled release includes EI's hi-level",
      "properties": {
        "ocid": "",
        "compiledRelease": {"$ref": "#/models/ei"}
      }
    }
  ]
}

```


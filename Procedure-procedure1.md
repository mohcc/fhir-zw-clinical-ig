# Example Procedure (Malaria RDT) - Zimbabwe Clinical IG v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Example Procedure (Malaria RDT)**

## Example Procedure: Example Procedure (Malaria RDT)

Profile: [Zimbabwe Procedure](StructureDefinition-zw-procedure.md)

**status**: Completed

**code**: Malaria rapid diagnostic test (RDT)

**subject**: `zw-patient-example`

**encounter**: `encounter1`

**performed**: 2026-05-01

### Performers

| | |
| :--- | :--- |
| - | **Actor** |
| * | `practitioner1` |

**location**: `location1`

**reasonReference**: [Condition Unspecified malaria](Condition-condition1.md)



## Resource Content

```json
{
  "resourceType" : "Procedure",
  "id" : "procedure1",
  "meta" : {
    "profile" : ["http://mohcc.gov.zw/fhir/clinical/StructureDefinition/zw-procedure"]
  },
  "status" : "completed",
  "code" : {
    "text" : "Malaria rapid diagnostic test (RDT)"
  },
  "subject" : {
    "reference" : "zw-patient-example"
  },
  "encounter" : {
    "reference" : "encounter1"
  },
  "performedDateTime" : "2026-05-01",
  "performer" : [{
    "actor" : {
      "reference" : "practitioner1"
    }
  }],
  "location" : {
    "reference" : "location1"
  },
  "reasonReference" : [{
    "reference" : "Condition/condition1"
  }]
}

```

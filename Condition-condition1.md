# Example Condition (Malaria) - Zimbabwe Clinical IG v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Example Condition (Malaria)**

## Example Condition: Example Condition (Malaria)

Profile: [Zimbabwe Condition](StructureDefinition-zw-condition.md)

**clinicalStatus**: Active

**verificationStatus**: Confirmed

**category**: Encounter Diagnosis

**code**: Unspecified malaria

**subject**: `zw-patient-example`

**encounter**: `encounter1`

**onset**: 2026-05-01

**recordedDate**: 2026-05-01

**recorder**: `practitioner1`



## Resource Content

```json
{
  "resourceType" : "Condition",
  "id" : "condition1",
  "meta" : {
    "profile" : ["http://mohcc.gov.zw/fhir/clinical/StructureDefinition/zw-condition"]
  },
  "clinicalStatus" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/condition-clinical",
      "code" : "active",
      "display" : "Active"
    }]
  },
  "verificationStatus" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/condition-ver-status",
      "code" : "confirmed",
      "display" : "Confirmed"
    }]
  },
  "category" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/condition-category",
      "code" : "encounter-diagnosis",
      "display" : "Encounter Diagnosis"
    }]
  }],
  "code" : {
    "coding" : [{
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "B54",
      "display" : "Unspecified malaria"
    }]
  },
  "subject" : {
    "reference" : "zw-patient-example"
  },
  "encounter" : {
    "reference" : "encounter1"
  },
  "onsetDateTime" : "2026-05-01",
  "recordedDate" : "2026-05-01",
  "recorder" : {
    "reference" : "practitioner1"
  }
}

```

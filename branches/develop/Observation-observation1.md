# Example Observation (Body Weight) - Zimbabwe Clinical IG v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Example Observation (Body Weight)**

## Example Observation: Example Observation (Body Weight)

Profile: [Zimbabwe Observation](StructureDefinition-zw-observation.md)

**status**: Final

**category**: Vital Signs

**code**: Body weight

**subject**: `zw-patient-example`

**effective**: 2026-05-01

**performer**: `practitioner1`

**value**: 70 kg (Details: UCUM codekg = 'kg')



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "observation1",
  "meta" : {
    "profile" : ["http://mohcc.gov.zw/fhir/clinical/StructureDefinition/zw-observation"]
  },
  "status" : "final",
  "category" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/observation-category",
      "code" : "vital-signs",
      "display" : "Vital Signs"
    }]
  }],
  "code" : {
    "coding" : [{
      "system" : "http://loinc.org",
      "code" : "29463-7",
      "display" : "Body weight"
    }]
  },
  "subject" : {
    "reference" : "zw-patient-example"
  },
  "effectiveDateTime" : "2026-05-01",
  "performer" : [{
    "reference" : "practitioner1"
  }],
  "valueQuantity" : {
    "value" : 70,
    "unit" : "kg",
    "system" : "http://unitsofmeasure.org",
    "code" : "kg"
  }
}

```

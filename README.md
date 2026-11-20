# Mini-KIS Interoperability Lab (FHIR R4, HL7 v2, IHE & Mirth)
Practical interoperability lab using synthetic test data ("Max Mustermann") and public test/validation environments (no real patient data or production systems):

- Patient Identity (PIX / PDQm style): SQLite cross-reference mapping KIS, LAB, and RAD IDs to a global patient ID; HAPI FHIR R4 Patient creation (201) and demographic search (200) illustrating multi-identifier resolution.
- Document Exchange (MHD style): FHIR DocumentReference creation (201) with LOINC, confidentiality, and SNOMED CT facility metadata, plus patient/status search (200).
- Audit Trail (ATNA / BALP style): FHIR AuditEvent logging patient record read access (201).
- IHE Gazelle EVS Validation: Validated HL7 v2 ITI-31 (ADT^A01 error resolution to PASSED; ADT^A40 PASSED) and XDS.b ITI-41 request metadata (PASSED) with public report OIDs.
- Interface Engine (Mirth Connect 4.5.2): Local HL7v2-to-FHIR channel (TCP Listener to HTTP Sender destinations) in progress (source and Destination 1 verified; Destination 2 error under analysis).

# PCC.ODH
Occupational Data for Health (ODH)

CI build -- https://build.fhir.org/ig/IHE/PCC.ODH/branches/master/index.html

- CI build failure log -- https://build.fhir.org/ig/IHE/PCC.ODH/branches/master/build.log

# Forked

This IG is forked from the USA specific IG from HL7 -- https://hl7.org/fhir/us/odh/

This fork is authorized by XXXXXX (Andrea, please put in evidence as to why IHE is allowed to fork HL7)

The following changes

- change to International
- change to IHE publisher
- change to IHE configuration parameters
  - canonical root
- Remove dependency on US-Core
- remove meta bread crumbs
- remove narratives, allow publisher to create narratives
- add ILO vocabulary valuesets for industries and occupations
  - use of these vocabularies in profiles
- remove forbiddance of effective[x] in PastOrPresentJob and RetirementDate as it is recommended by FHIR core to have effective[x] and there is no good rational

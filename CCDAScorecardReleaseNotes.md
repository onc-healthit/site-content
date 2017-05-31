#### Release Notes

* Updates included in the **SITE 3.1.4 03/31/2017 Release** for the **C-CDA Scorecard 'R1.1'**

  * Improvements
    * Removed technical error messages in "One Click" PDF when schema errors are returned
    * Removed Industry Average from UI header and redesigned for readability of top-level results
    * When effectiveTimes are specified with nullFlavor, the following rules are no longer applied as we cannot compare an effectiveTime value with an unknown:
      * Rule: Effective Date/Times for all historical activities should be within the lifespan on the patient
      * Rule: Allergies observation effectiveTime should align with Allergies concern act effectiveTime
      * Rule: The Effective Date/Time elements for the Result Organizer must encompass the underlying observations
  
  * Fixes
    * The Scorecard no longer validates displayNames for codeSystems that Scorecard does not maintain in its repository. The Scorecard repository maintains the following codeSystems.
      * SNOMED-CT
      * LOINC
      * ICD9CM_DX
      * ICD9CM_SG
      * ICD10CM
      * ICD10PCS
      * RXNORM
      * CPT-4
      * CVX

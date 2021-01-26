
Upcoming Updates:

Release 3.1.44 (Targeted for 02/22/2020)
* C-CDA Validator enhancements and bug fixes.

Completed Updates:
* C-CDA Validator
  * Fix issue requring 0 provenance (author) instances 
  * Update birth sex and telecom validation to fire error for cures and warning for non-cures
  * Fix birth sex and telecom validation not firing relevant issues when severity is set to errors only      
  * Fix scenario file for Cures selecting pre-cures scenarios in SITE C-CDA Validator UI
* Scorecard  
  * Identify and parse the negation indicator ( eg : negationInd=”true” ) element CCDA files
  * Fix the scorecard rules (where applicable) to not apply the rule when negInd value is true
    * Rules that are impacted:
      * Problem Concern effective times reflect the appropriate problem concern status
      * Allergy Concern observation effective times reflect the appropriate allergy concern status
      * Medications coded with RxNorm SCD, SBD, GPCK, or BPCPK codes
      * Systems should capture birth sex independent of the Administrative Gender and encode them as an observation in the Social History Section
      * Each medication needs to have its own Medication Signature Text EntryRelationship and this reference should exist in the same section found
      * Fix in UCUM unit rule: Rule not to be applied for xsi:type = "REAL"
      * Lab Result values should use preferred UCUM units  

Release 3.1.43

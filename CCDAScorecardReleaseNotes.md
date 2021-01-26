#### Release Notes
* Updates included in the **01/25/2021 Release** for the **C-CDA Scorecard 'R2.4'**
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

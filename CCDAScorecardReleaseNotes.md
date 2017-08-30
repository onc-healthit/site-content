#### Release Notes
* Updates included in the **SITE 3.1.7 08/29/2017 Release** for the **C-CDA Scorecard 'R1.4'**

* Updates to Rules:
  * Enhancement to Rule: Each entry should have a text reference that is linked to the narrative text in the section.  
"Each entry has to be linked to related narrative text. For each entry, a text element has to be contained with a reference back to the Section/text element. Sometimes the entry/text element may be absent and the code/originalText element would be used to perform the linking. This rule is applied to each of the EntryRelationship underneath the top level entry."
  * Relaxation of Time element to YEAR in case of Allergies and Problems.
  * Relaxation of Time element to DAY in case of Medications and Immunizations.
  * Updates to "Allergies observation effective time should align with Allergies concern act effective time".
    * The new implementation will be checking: If the AllergyConcern/status is active, there cannot be a value in the high element of the observation/effective time, if the AllergyConcern/status is Resolved/Inactive then the high element should be present with a value.
  * Removed the implementation of the following rules from Problems Section:
    * The EffectiveDate/Time elements for the Problem Concern Act must encompass the underlying observation
    * Problem Concern status and Problem Observation status are consistent with each other
  * Updates to the rule below in Problems Section:
    * Problem Concern effective times reflect the appropriate problem concern status. Changed the existing implementation to: If the ProblemConcern is Active, at least one of the Problem Observations underneath it cannot contain a value in the high time. If the ProblemConcern is Resolved/Inactive, the ProblemObservation/EffectiveTime should contain a value in the high element.

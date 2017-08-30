#### Release Notes
* Updates included in the **SITE 3.1.7 08/29/2017 Release** for the **C-CDA Scorecard 'R1.4'**

Updates to Rules Implementation:
 
1. Enhancement to Rule: Each entry should have a text reference that is linked to the narrative text in the section.  
"Each entry has to be linked to related narrative text. For each entry, a text element has to be contained with a reference back to the Section/text element. Sometimes the entry/text element may be absent and the code/originalText element would be used to perform the linking. This rule is applied to each of the EntryRelationship underneath the top level entry."      

2. Relaxation of Time element to YEAR in case of Allergies and Problems.
3. Relaxation of Time element to DAY in case of Medications and Immunizations.
4. Updates to "Allergies observation effective time should align with Allergies concern act effective time".
   - The new implementation will be checking  If the AllergyConcern/status is active, there cannot be a value in the high element of the        observation/effective time, if the AllergyConcern/status is Resolved/Inactive then the high element should be present with a value.
5. Removed the implementation of following rules from Problems Section
     • The EffectiveDate/Time elements for the Problem Concern Act must encompass the underlying observation.
     • Problem Concern status and Problem Observation status are consistent with each other
6. Updates to below rule in Problems Section.
    Problem Concern effective times reflect the appropriate problem concern status.
   Changed the existing implementation to: If the ProblemConcern is Active, then at least one of the Problem Observations underneath          cannot contain a value in the high time. If the ProblemConcern is Resolved/Inactive, then the ProblemObservation/EffectiveTime 
   should contain a value in the high element.


	

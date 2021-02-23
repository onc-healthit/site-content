
Upcoming Updates:

Release 3.1.45 (Targeted for 03/29/2020)
* C-CDA Validator enhancements and bug fixes.

Completed Updates:
* C-CDA Validator
	* Content Validation
		* Allow exception for including Smoking Status data when the scenario has none if Smoking Status value/@code is equal to SNOMED-CT code 266927001 "Unknown if ever smoked"
		* Fix crash when parsing a code element in the Birth Sex Observation template which has no code attribute
		* Update JDK
	* Vocabulary Validation
		* Update JDK
	* MDHT/IG Validation
		* Fix incorrect root for UDI Device Identifier Observation value causing invariant violation parsing error
		* Update MDHT to the latest build: https://github.com/mdht/mdht-models/releases/tag/v20210210
		* Update JDK 
	* Test data updates
		* Updated Telecom Email to not mandate the "use" attribute
		* Update Allergy Drug Class to a code present in the ValueSet
		* Updated Vital Signs to include appropriate Weight and Height for BMI calculations 
		* Added Note to indicate Provenance is only for USCDI data elements
		* Added Note to indicate Provenance Timestamp can be changed by working with the ATL
		* Corrected Participant codes for Care Team Members
		* Removed Provenance from Authors related to Non USCDI data classes and elements
* Scorecard
	* Relax the rule on Effective time when time is not specified.
	* A valid YYYYMMDD is an acceptable format.
   	* NullFlavor  should not be tagged as error in EffectiveTime Precision Rule.
   	* Fix Problem Concern Status Rule where it is getting triggered for wrong template ID.
   	* Fix Allergy Concern Status Rule to not consider Aborted status for the rule validation.

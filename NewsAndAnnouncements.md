
Upcoming Updates:

Release 3.1.45 (Targeted for 03/29/2020)
* C-CDA Validator enhancements and bug fixes.

Completed Updates:
* C-CDA Validator
	* Content Validation
		* Allow exception for including Smoking Status data when the scenario has none if Smoking Status value/@code is equal to SNOMED-CT code 266927001 "Unknown if ever smoked"
		* Fix crash when when parsing a code element in the Birth Sex Observation template which has no code attribute
		* Update JDK
	* Vocabulary Validation
		* Update JDK
	* MDHT/IG Validation
		* Fix incorrect root for UDI Device Identifier Observation value causing invariant violation parsing error
		* Update JDK 
* Scorecard
   * Relax the rule on Effective time when time is not specified. A valid YYYYMMDD is an acceptable format.
   * NullFlavor  should not be tagged as error in EffectiveTime Precision Rule.
   * Fix Problem Concern Status Rule where it is getting triggered for wrong template ID.
   * Fix Allergy Concern Status Rule to not consider Aborted status for the rule validation.

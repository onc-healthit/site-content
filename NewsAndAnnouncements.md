
Upcoming Updates:

Release 3.1.47 (Targeted for 05/31/2021)
* C-CDA Validator enhancements and bug fixes.

Completed Updates:
* C-CDA Validator
	* Content Validation
		* Include provenance representedOrganization reporting where applicable to properly clarify error output messages
		* Fix provenance checking in Notes Entry to account for time zones     
	* Test data updates
		* Updated Care Team Validation as per the Companion Guide
		* Updated Pediatric Vitals Error Message to consult ATL when different results are obtained 
		* Updated Sample 3 files for Inpatient criteria to include Henry Seven as Attending Physician Care Team Member
		* Updated VDT Xml samples Health Concerns Section to point to Problem Section using right identifiers
	* Code Validation (CURES validator only)
		* Updated CPT code system Files to CPT 2021 Data File_PLA Q2 Updt
			* Now uses the correct long name file per the ReadMe.txt found in the Code Validator API Project documentation
		* Updated CPT loader to accommodate the tab format of the LONGULT.txt file

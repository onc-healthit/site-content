
Upcoming Updates:

Release 3.1.46 (Targeted for 04/26/2021)
* C-CDA Validator enhancements and bug fixes.

Completed Updates:
* C-CDA Validator
  * Updated Happy Kid Vitals test data to reflect the CDC growth charts more accurately.
  * Updated the test data sample 3 files for both inpatient and ambulatory to more clearly identify USCDI data elements.
  * In the software side, Added tolerance based validation for growth charts to allow for variations by EHR vendors.
  * Updated Gold Sample with cures data.
  * Fix blank Organization Name in Provenance error output.
  * Fix rejection of a submitted Provenance time which is not matching the scenario time exactly. Instead, the base-level-date is enforced but the time and time-zone can be any value, if formatted correctly.
  * Add Provenance date and time/time-zone validation.
* Scorecard  
  * Update XML Issue line number results to a pretty-printed output.
  * Update Scorecard API documentation and GitHub readme to use ccda.healthit.gov domain.

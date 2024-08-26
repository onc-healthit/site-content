# The Standards Testing & Implementation Environment (SITE)

## Release Notes

### 3.1.82 | Released on 8/26/2024

* [ett](https://github.com/onc-healthit/ett) updated to version [2.3.70](https://github.com/onc-healthit/ett/releases/tag/2.3.70)
  * Update log4j version (SITE-4191)
* [reference-ccda-validator](https://github.com/onc-healthit/reference-ccda-validator) updated to version [1.0.75](https://github.com/onc-healthit/reference-ccda-validator/releases/tag/1.0.75)
  * Updates to mdht version
* [content-validator-scenarios](https://github.com/onc-healthit/content-validator-scenarios) updated to version [1.0.1](https://github.com/onc-healthit/content-validator-scenarios/releases/tag/1.0.1)
  * SDOH goal code updated to 161036002
* [content-validator-api](https://github.com/onc-healthit/content-validator-api) updated to version [1.0.56](https://github.com/onc-healthit/content-validator-api/releases/tag/1.0.56)
  * Related Person TemplateIds Comparison
* [FHIR Tools](https://github.com/onc-healthit/fhir-tools) updated to version [1.0.1](https://github.com/onc-healthit/fhir-tools/releases/tag/1.0.1)
  * Dependabot dependency update for FHIR R4
  * Update README.md


### 3.1.81 | Released on 7/29/2024
* [ett](https://github.com/onc-healthit/ett) updated to version [2.3.69](https://github.com/onc-healthit/ett/releases/tag/2.3.69)
* [ccda-scorecard](https://github.com/onc-healthit/ccda-scorecard) updated to version [2.7.1](https://github.com/onc-healthit/ccda-scorecard/releases/tag/2.7.1)
* [reference-ccda-validator](https://github.com/onc-healthit/reference-ccda-validator) updated to version [1.0.74](https://github.com/onc-healthit/reference-ccda-validator/releases/tag/1.0.74)
* [content-validator-api](https://github.com/onc-healthit/content-validator-api) updated to version [1.0.55](https://github.com/onc-healthit/content-validator-api/releases/tag/1.0.55)

### SITE V3.1.80 | Released on: 06/24/2024
* Reference-ccda-calidator to 1.0.73
  * Update MDHT assessment scale supporting observation to allow values other than "CD"
* ETT to 2.3.6
  * Update FAQ to remove "2015" and "2015 Edition" from title of links
* Scorecard to 2.7.0
  * Update jackson to 2.17.1
  * Update postgresql driver to 42.7.3
* FHIR Tools to 1.0.0
  * Update dependencies of bulkr4, r4

### SITE V3.1.79 | Released on: 06/03/2024
* C-CDA Validator
  * Update MDHT per 2018 and later errata
  * Update ReadMe to remove public API references and add keycloak properties
  * Fix USCDIv3 referral error
  * Fix USCDIv3 goals and health concerns error
  * Fix health concern observation code in MDHT
* ETT
  * Fix reference validator API call that broke scenario testing
  * Fix download button in USCDIv3 validator
  * Remove reference to "2015 Edition Cures Update"

### SITE V3.1.78 | Released on: 04/29/2024
* ETT
  * Remove Cures Update references from USCDI v2 and v3 scenario files
  * C-CDA Validators - Removed need to use c-cda objectves text file
  * Updated b1 Negative testing files to reference USCDI instead of CCDS
* SITE
  * Update Test Data File titles and introduction to remove 2015/Cures Update.
  * Removed USCDIv2  
* C-CDA Validator
  * Correct a typo in Hunger Vital Assessment Code in Newman and Larson Data sets

### SITE V3.1.77 | Released on: 03/25/2024
* ETT
  * Update SVAP buttons b1, h1 and h2 to point to USCDIv3 instead of v2
* SITE
  * Update URL in Scorecard API documentation
* C-CDA Validator
  * USCDIv3 vocabulary added validation for Gender Identity, Sexual Orientation and Specimen Type.

### SITE V3.1.76 | Released on: 02/26/2024
* ETT
  * UI language updates to Validator Home page
  * Removed USCDI v2 option from Direct Testing Home C-CDA Validator dropdown
  * Direct: UI Updates for send/receive messages with various ECDSA signatures
* SITE
  * Enable Keycloak
* C-CDA Validator
  * Update 170.315_b1_toc_amb_svap_uscdiv2_sample1.xml to fix SDOH error

#### SITE V3.1.75 | Released on: 01/29/2024
* ETT
  * Fix for GG issue granular race checking in b.1 - Alice Newman
  * Remove reference of 2015 Edition/Cures Update from tools
  * UI Table update for USCDIv3
* SITE
  * Remove reference of 2015 Edition/Cures Update from tools
* C-CDA Validator
  * Fix defects for RelatedPerson
  * Updated USCDIv3 content validation for RelatedPerson, Specimen and Socialhistory observations 

#### SITE V3.1.74 | Released on: 12/18/2023
* C-CDA Validator
  * Improve C-CDA R1.1/MU2 Validator uptime
  * Remove more granular race code with unpopulated data
* ETT
  * Added USCDI v3 C-CDA Validator
* SITE
  * Added USCDI v3 C-CDA Validator

#### SITE V3.1.73 | Released on: 11/27/2023
* C-CDA Validator
  * Apply fix for ETT GG: "Patient Kid,Happy Chest X-ray completed before birth"
  * Apply fix for ETT GG: "Community Health and Hospitals"
  * Improve R2.1/USCDI C-CDA Validator uptime
* ETT
  * Add Clear pass/fail indicators in the XDR Test Cases
  * Update SVAP 2022 to USCDI v2
* SITE
  * Update SVAP 2022 to USCDI v2

#### SITE V3.1.72 | Released on: 10/30/2023
* C-CDA Validator
  * Add public API usage to readme
* ETT
  * Resize document search window to resolve truncated document names
  * Add submit button inside document search window
  * Update separate clientId and key for Keycloak
  * Add link for SVAP standards versions to validator home page
* SITE
  * Update separate clientId and key for Keycloak
  
#### SITE V3.1.71 | Released on: 09/25/2023
* C-CDA Validator
  * Update Ambulatory and Inpatient Test Data Sample 1 for b1, e1 and g9 criteria to remove Lab Narrative for USCDIv2
  * Update Ambulatory Test Data Sample 1 for b1, e1 and g9 criteria to change goal observation code for USCDIv2
  * Update Ambulatory Test Data Sample 1 for b1, e1 and g9 criteria to fix health concern code in test data to match companion guide for USCDIv2
  * Update Ambulatory Test Data Sample 1 for b1, e1 and g9 criteria to make clinical test result optional for EKG tests for USCDIv2
  * Fix errors in Reference C-CDA validation for Inpatient samples 1 and 3 for b1, e1 and g9 for USCDIv2
  * Change Reference C-CDA validation to allow additional data such as procedures, lab results, etc. which may not be present in the scenario as requested by the vendors
  * Add svap2023 flag to Reference C-CDA Validator API. Note: There is NO implementation logic/support for SVAP 2023 validation yet. This is a work in progress update
* ETT
  * Update sender/receiver buttons to ensure they depress on selection
  * Replace static variables in upload controller

#### SITE V3.1.70 | Released on: 08/28/2023
* Reference C-CDA Validator WAR
  * Removed SHALL constraint for Nonexistent id Requirement in Section Time Range Observation
  * Fixed incorrect error for Informant RelatedEntity
* SITE
  * Updated SITE/test-tools section to remove non functional links
* C-CDA
  * Update scenario files language in word document to match pdf scenarios
  
#### SITE V3.1.69 | Released on: 07/31/2023
* C-CDA Validator
  * Soft-deploy Keycloak for C-CDA Scorecard API access
* ETT
  * Update JSON and File Upload dependencies
  * Fix XDM Validator not displaying Pass/Fail Status
  * Remove direct link to announcement page
  * Correct home phone value in 170.315_b9_CP_Amb scenario file
* FHIR
  * Address Google Groups issue, "FHIR server returns 500 on querying example url" via update to 404 as per hl7 documentation and update to links
* General
  * Update Infrastructure

#### SITE V3.1.68 | Released on: 06/26/2023
* C-CDA Validator  
  * Soft-deploy Keycloak for Reference C-CDA Validator Service API access
  * Fix Google Group issue, "SVAP Message Validator - Goal LOINC"
  * Fix Google Group issue, "routeCode translation displays as not an active code"
* ETT
  * Remove announcement page from UI
  * Fix JSONObject Text error for ETT C-CDA Validator
  * Fix error message for ETT C-CDA Validator if RefVal service is down
  * Update error message for excessively large files for ETT C-CDA Validator
* General
  * Infrastructure updates

#### SITE V3.1.67.1 | Released on: 05/08/2023
* C-CDA Validator
  * Update Test Data scenario files to ensure SVAP 2022 USCDI v2 criteria is being applied properly for Inpatient scenarios
  * Correct Gender Identity Extension in scenario files
  * Fix incorrect code system OID in scenario files
  * Update EffectiveTime checking in PlannedProcedure to allow specification of high value even if not present in scenario
  * Fix XDR Submit scenarios to send Negative Testing files
  * Remove erroneous procedures from scenario files
  * Remove Discharge Disposition codes from Ambulatory samples

#### SITE V3.1.67 | Released on: 04/24/2023
* C-CDA Validator
  * Further improve memory handling to address recent downtime issues 
  * Change §170.315(b)(2)(iv) language in test data to clarify that the output file is to be in a CCD format. Update: "The SUT should then generate a C-CDA (using the CCD template in C-CDA Release 2.1) that contains the Allergies, Medications and Problems from the two Referral Notes that were provided." 
* General
  * Implement security updates in infrastructure

#### SITE V3.1.66 | Released on: 03/27/2023
* C-CDA Validator
  * Resolve ETT Google Groups thread, "Vocabulary Errors for birthplace address"
  * Improve memory handling
* ETT
  * Remove SVAP 2022 DCDT from Cert Discovery drop down
  * Remove broken links in 2015 Direct Certificate Discovery Tool page
* General
  * Infrastructure updates

#### SITE V3.1.65 | Released on: 02/27/2023
* C-CDA Validator
  * Update SubstanceReactantForIntolerance value set to include the latest codes from VSAC 	
* Direct
  * Fix drop downs not loading for "Select a Discovery Test Case"
  * For Direct: 4.0, add ability to send a direct message using a certificate that does not have a CRL
* General
  * Infrastructure updates
  
#### SITE V3.1.64 | Released on: 01/09/2023
* Direct
  * Add Direct version 1.3 to ETT
  * Add SVAP 2022 DCDT to ETT
* Other
  * Fix broken links in SITE test-tools page

#### SITE V3.1.63 | Released on: 12/05/2022
* C-CDA Validator
  * Add table explanation to the ETT validator home which relates certification criteria version with C-CDA and USCDI version: https://ett.healthit.gov/ett/#/validators
* FHIR
  * R4 dependency update for bulk R4
* Other
  * Various Direct and other server infrastructure upgrades and fixes
  * Fix ETT GG issue, "XDR Endpoint with TLS not working"

#### SITE V3.1.62 | Released on: 09/29/2022
* C-CDA Validator
  * Correct template versions for Problem Status and Allergy Status to 2019-06-20
  * Relax severity of value set constraint on Provenance Author Participation to match IG
  * Update scenarios for SVAP-2022 to match test data for inpatient samples
* FHIR
  * Update navigation links in R4 Bulk data pages
  
#### SITE V3.1.61 | Released on: 08/31/2022
* C-CDA Validator
  * Release the new C-CDA R2.1 Validator for 2015 Edition Cures Update and SVAP 2022 on SITE, ETT, and within the Reference C-CDA Validator WAR
    * Includes new test scenario files and test data files (https://github.com/onc-healthit/2015-edition-cures-update-uscdi-v2-testdata)
  * Update vocabulary to the July 2022 VSAC release
  * Resolve ETT Google Groups thread, "Pregnancy Observation for Possible Pregnancy or Not Pregnant" by adding the new codes to the Extended Pregnancy Status Value Set 2.16.840.1.113762.1.4.1099.24 DYNAMIC
  * Resolve ETT Google Groups thread, "Result referenceRange validation error when the requirements are met" by adding support for IVL_REAL
  * Resolve ETT Google Groups thread, "ETT bug validating Care Team Member Act?" by relaxing Care Team Member Act participant conformance rule to a MAY vs a SHALL severity
  * Resolve ETT Google Groups thread, "170.315(b)(9) – Care Plan_Phone Number Issue"
  * Improve Artifactory up time for local builds
  * Fix MDHT 20220126 release by uploading the missing org.hl7.security.ds4p.contentprofile-3.0.0.20220126.jar into the MDHT_CCDA_R2.1_R1.1_MU2_DS4P_20220126_build.zip release artifact 
* Scorecard
  * Update C-CDA parser  dependency to match content-validator-api capabilities
* FHIR
  * Update dependencies
  * Update bulk Data API link to (https://fhirsandbox.healthit.gov/clientbulkr4)
* General
  * Increase C-CDA server uptime potential
  * Update ETT dependencies
  * Update SITE dependencies

#### SITE V3.1.60 | Released on: 07/25/2022
* C-CDA Validator
  * Implement Appendix A and B, C-CDA Templates from Clinical Notes STU Companion Guide, Release 3 US Realm, May 2022
  * Include Appendix A and B update in C-CDA R2.1 Cures Update Validator within SITE and ETT UIs as USCDI Version 2 Beta
  * Reference external Docker setup option in the Reference C-CDA Validator readme (relevant to local instantiation)
  * Update Artifactory, the public repository for Reference C-CDA Validator dependencies (relevant to local instantiation)
  * Separate Reference, Content, and Code logs (relevant to local instantiation)
* Scorecard
  * Update dependencies
* Scorecard Batch
  * Update dependencies
* FHIR
  * Update dependencies
* General
  * Update server infrastructure

#### SITE V3.1.59 | Released on: 05/31/2022
* C-CDA Validator
  * Improve validator backend service uptime
  * Further improve Artifactory uptime (C-CDA dependency server)
* FHIR
  * Fix incompatible character encodings UTF-8 and ASCII-8BIT for US Core Encounter Profile 
  * Update dependencies Spring, Spring-security-web, and JUnit
  * Remove FHIR Query Tool and FHIR Conformance Test Tool

#### SITE V3.1.58 | Released on: 04/25/2022
* C-CDA Validator
  * Update CIRI (b2) test data instructions and test data xml files to allow the reconciliation of Patient birth names appropriately 
  * Add DS4P jars to MDHT build scripts for future builds/releases
  * Increase Artifactory server uptime to enhance Reference C-CDA Validator builds
* Scorecard
  * Update API Content URL on Scorecard Batch Application instructions and config data 
* FHIR
  * Update fhir_server_url for FHIR tools from 'https://fhirsandbox.healthit.gov/secure' to 'https://fhirsandbox.healthit.gov/secure/r4'
  * Add support elements: status, category, category.coding, category.coding.system for Bulk R4 Observation resources
  * Add support elements: status, category, code, subject, effective, issued, performer, result for Bulk R4 DiagnosticReport resources 
* General
  * Mitigate various server issues and harden for future releases

#### SITE V3.1.57 | Released on: 03/28/2022
* C-CDA Validator
  * Update value set 2.16.840.1.113883.3.88.12.80.62 Vital Sign Result Type to the latest version in order to allow the use of code 3150-0
  * Update test data to change Allergy Drug Class to a value in the Value set for b1, e1, g9 criteria. The sender pdf files have been updated
  * Update CIRI (b2) test data instructions to allow the reconciliation of an Allergy due to a drug class
* FHIR
  * Update R4 CapabilityStatement with absolute URLs if they are not fragment references (/fhir/metadata) 

#### SITE V3.1.56 | Released on: 02/28/2022
* C-CDA Validator
  * Add regulation clarification to configuration
  * Fix ActStatus Value Set OID in configuration from 2.16.840.1.113883.1.11.159331 to 2.16.840.1.113883.1.11.15933
* General
  * Update server infrastructure
* FHIR
  * Remove reference to STU3 and reference to DSTU2 from fhirsandbox
* ETT to 2.3.43
  * Update metadata for XDM in SMTP 28/29

#### SITE V3.1.55 | Released on: 01/31/2022
* C-CDA Validator
  * Apply STU-1981
	* Fixed errata on Lot or Batch Number observation to support ED versus ST
	* https://jira.hl7.org/browse/CDA-1981
  * Add missing SDTC extension sdtc:text and implementation on organizer
  * Add support for IVL_REAL datatype and implementation on organizer
* General
  * Update server infrastructure
* FHIR
  * Update FHIR R4 Spring dependency to 5.1.13.RELEASE

#### SITE V3.1.54 | Released on: 12/27/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Update linked reference mismatched org name message for clarity and specificity
  * Fix recent server configuration issue which may have suppressed certain vocabulary results
  * Add missing CDA Extensions from 2018: sdtc:asPatientRelationship, sdtc:deceasedInd, sdtc:deceasedTime, sdtc:multipleBirthInd, sdtc:multipleBirthOrderNumber, sdtc:statusCode and stdc:desc
  	* See https://confluence.hl7.org/display/SD/CDA+Extensions for a detailed description of the extensions
  * Limit Vital Sign Observation/value to data type PQ
  * Update value set for Marital Status to include U: Unmarried and C: Common Law
  * Report only one validation issue (versus two issues) for an incorrect or missing Allergy Section Code

#### SITE V3.1.53 | Released on: 12/06/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Enforce provenance templateId and extension requirements at a stricter level for content comparisons
  * Fix potential provenance null pointer exception
* C-CDA Parser (for C-CDA Scorecard)
  * Fixed bug in parsing encompassingEncounter element
* FHIR
  * Added support for system/Patient.read scope for Bulk R4
  * Fixed: R4 US Core - CapabilityStatement.id must match Regex: [A-Za-z0-9\-\.]{1,64}
  * Fixed: Provenance resources must support elements: agent.type, agent.type.coding.code: author, agent.type.coding.code: transmitter
* ETT to 2.3.40
  * Fix potential security issues in ETT
 
#### SITE V3.1.52 | Released on: 10/25/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Require provenance identification using templateId for provenance TS validation
  * Fix configuredExpression totals by severity in production by enabling dynamic vocab
  * Implement errata CDA-2008 https://jira.hl7.org/browse/CDA-2008 which relaxes NoteActivity/code/translation requirement to a SHOULD vs a SHALL: Consol Note Activity SHALL contain exactly one [1..1] code (3250-16895)/@code="34109-9" Note (CodeSystem: 2.16.840.1.113883.6.1 LOINC) (3250-16940, 3250-16941) code SHOULD contain zero or more [0..*] translation, which SHOULD be selected from ValueSet NoteTypes 2.16.840.1.113883.11.20.9.68 STATIC 20191017
  * Fix inheritance bug in Medications Section where an error in both entries optional and required is reported, instead of reporting required only
  * Fix patient name elements for b2 CIRI ambulatory scenario files
  * Fix parsing bug where Procedures/NoteActivity is mistaken for ProcedureActivityProcedure
  * Update the following value sets to the latest published version: CVX Vaccines Administered Vaccine Set and Substance Reactant for Intolerance
  * Add newly available value sets: Transmission Based Precaution Types, Organism, Microbiology and Antimicrobial Susceptibility Tests, and Infectious Disease
* MDHT
  * Release https://github.com/mdht/mdht-models/releases/tag/v20211021 and incorporate it into the Reference C-CDA Validator
* ETT
  * Apply various security updates
* FHIR
  * AllergyIntolerance added support for elements: reaction, reaction.manifestation
  * Fix incompatible character encodings UTF-8 and ASCII-8BIT for Inferno Test BDGV-08
* C-CDA Parser (for C-CDA Scorecard)
  * Enable Async

#### ETT V2.3.38.2 | Released on: 10/13/2021
* Fix potential security issues in ETT

#### ETT V2.3.38.1 | Released on: 9/27/2021
* Fix potential security issues in ETT

#### SITE V3.1.51 | Released on: 09/27/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Relax participant constraints to allow free-text names in Referral Note as part of new MDHT 20210924 Release
  * Update 170.315(e)(1) Inpatient setting Sample 1 files to include Reason for Referral instructions to enable vendors to create Referral Notes
* SITE-UI
  * Fix 'Original C-CDA' tab display issue in CURES SITE C-CDA Validator
* ETT to 2.3.38
  * Update ETT dependencies as per dependabot
  * Fix potential SQL injection issues in ETT

#### SITE V3.1.50 | Released on: 08/30/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Fix DocumentBuilderFactory XXE vulnerability
  * Fix exception during parallel execution of DocumentBuilder
  * Update to support HL7 Datatype IVL_REAL as part of new MDHT 20210824 Release
* SITE-UI
  * Fix direct message sender UI sent and received time stamps
* Scorecard
  * Fixed encompassingEncounter efferctiveTime parsing issue
* FHIR Sandbox Updates
  * Added new Patient Data set
   
#### SITE V3.1.49 | Released on: 07/26/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Add linked reference support for Note Activity
  * Implement Errata 2041: Allow for Advance Directive organizer or Advance Directive observation in an Advance Directive section but prevent an entry from having both an     observation and an organizer
  * Update ValueSet HL7 RefrainPolicy 2.16.840.1.113883.1.11.20446 to reflect the DS4P IG
  * Updated dependencies for security
* SITE-UI
  * Fix xdr message sender endpoint
 
#### SITE V3.1.48.1 | Released on: 07/02/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Add support for linked references in author when validating provenance representedOrganization/name (with the exception of Note Activity)
  * Remove XML files from e1 criteria for inpatient

#### SITE V3.1.48 | Released on: 06/28/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Remove XML Line number and XPath from Content Validation results 
  * Add logic to allow Notes Activities to be present in any section within the C-CDA document 
  * Relax Care Team section requirement to warnings instead of errors
  * Update Gold Samples for Sample1 and Sample2
  * Fix bug in the CPT Loader where some records were missing

#### SITE V3.1.47 | Released on: 06/02/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Updated Content Validator to allow notes activities in specific sections which include Lab Results, Procedures, Notes and Encounters
  * Updated Error Messages for Notes Provenance Entries
  * Updated Provenance Validation for Inpatient setting for Jane Clarkson to have the right organization name
  * Updated Sample1 and Sample2 files to include Clinical Notes validation

#### SITE V3.1.46 | Released on: 04/26/2021

#### C-CDA Sandbox Updates:
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

#### SITE V3.1.45 | Released on: 04/05/2021

#### C-CDA Sandbox Updates:
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

#### SITE V3.1.44.1 | Released on: 03/08/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
	* Content Validation
		* Fix invalid errors fired when more authors exist in the submitted data than the scenario
		* Add Note Activity enforcement to Results and Procedures Sections
		* Fix telecom issue for type mailto
	* Test data updates
		* Updated Vitals Test Data to reflect the CDC growth charts for pediatric vitals
		* Updated Validator to remove the provenance to non USCDI data elements
		* Updated Telecom values for CIRI b2 criteria for Telecom validation

#### SITE V3.1.44 | Released on: 02/22/2021

#### C-CDA Sandbox Updates:
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
* ETT to 2.3.31
    * Fix XDR 1 and XDR 2 tests to call the Cures validator when Cures files are selected with updated parameters.
    * Update XDR 7 and XDR 9 tests to pass when an exception is thrown.

#### SITE V3.1.43 | Released on: 01/25/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Fix issue requiring 0 provenance (author) instances 
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
* ETT to 2.3.30
  * Updated XDR 1 and XDR 2 tests to call the Cures validator when Cures files are selected.
  * Updated SMTP 8, 14, 18 test to call the Cures validator when Cures files are selected.
  
#### SITE V3.1.42 | Released on: 12/07/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Add IG-level UDI validation
  * Add Provenance content validation for section and entry relationships
  * Update CDT, CPT, LOINC, SNOMED, and RXNORM code systems
  * Fix Care Team cardinality and severity issues (4435-152, 4435-166, etc.)
  * Fix Note Types translation code issue where our value set was out of date (3250-16940, 3250-16941)
  * Fix cardinality and remove 'such that it' for Note Activity Author Participation (3250-16913)

#### SITE V3.1.41.1 | Released on: 11/16/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Updated value sets to the latest available from VSAC (for the CURES option)
  * Fixed telecom validation to validate numbers only
  * Fixed issue where the Reference Validator was not producing a log
  * Removed excess cache info and warnings from log
  * Updated JDK version notes in Reference Validator readme

#### SITE V3.1.41 | Released on: 10/27/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
   * Updated Vocabulary validator with the latest VSAC value sets. 
   * Based on MDHT build <https://github.com/mdht/mdht-models/releases/tag/v20201024> contains the following fixes:
    * Added Notes Templates
    * Added Care Team Template
    * Added Provenance Template
* Updated Content Validation and fixed defects associated with Notes and Provenance validation
* Scorecard
  * Fix missing logo, header and link images
  * Fix save report download bug and related broken links
  * Update environment configurations
  * Fix GlobalNamingResources not showing in readme
  
#### SITE V3.1.40 | Released on: 09/28/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Updated USCDI Sample 3 Test Data for Ambulatory and Inpatient to correct date of birth and timing errors.
  * Updated Notes Error reporting and fixed errors related to Sample 3 for Ambulatory and Inpatient settings.
  * Updated Author Provenance Error Reporting.
  * Changed Telecom and Birth Sex Error reporting from WARNING to ERROR.
* Scorecard
  * Resolve issues when parsing a document with multiple patient names where one does not have a legal use.
  * Update support email to edge-test-tool@googlegroups.com.
* ETT to V2.3.27
  * Fixed a bug on ETT to download cures CCDA files from GitHub.

#### SITE V3.1.37.1 | Released on: 09/15/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Renamed the test data files to start from version 1.
	 * Updated the test data to include USCDI elements as part of Sample3 files.
	 * Updated Sample3 for b1, e1 and g9.
	 * Updated DS4P test data to include entry level markings. 

#### ETT V2.3.25.1 | Released on: 8/13/2020
* Add endpoints documentation

#### ETT V2.3.25 | Released on: 8/5/2020
* Make MDN checks in MU2 39, 40 and 41 case insensitive.

#### SITE V3.1.37 | Released on: 06/29/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * DS4P update to the 'CURES' Reference C-CDA Validator 
    * Reviewed and updated DS4P validations based on HL7 Reaffirmation Status
  * Content-related cures updates to the 'CURES' Reference C-CDA Validator
    * Updated C-CDA Validator with changes to detect conformance to Notes sections and Notes entries for compliance to US CDI

#### SITE V3.1.36 | Released on: 06/01/2020

#### C-CDA Sandbox Updates:
* __Scorecard 2.0__ (Released on: 06/03/2020)
  * Support the latest rubrics/new Scorecard rules developed over the past year
  * Support CURES validation within the Scorecard
  * Update UI
* C-CDA Validator
  * Add 2015 Edition Cures Update R2.1 Validator support to the C-CDA Validator
  
#### ETT V2.3.24 | Released on: 6/1/2020
* Remove 2014 edition certification tools.

#### ETT V2.3.23 | Released on: 6/1/2020
* Add Cures Update C-CDA R2.1 Validator.

#### SITE V3.1.35 | Released on: 04/27/2020

#### C-CDA Sandbox Updates:
* Scorecard
  * Add grade comparison bar chart
  * Add IG, Vocabulary, and Issue checks count
  * Implement header redesign
  * Improve performance by 16.24%
  * Add disclaimer to R1.1 docs scored
* C-CDA Validator
  * Add dynamic issue count for total IG Conformance error checks to the API
  * Add vocabulary configuration error checks count to the API  

#### SITE V3.1.34 | Released on: 03/30/2020

#### C-CDA Sandbox Updates:
* None.

#### SITE V3.1.32 | Released on: 01/27/2020

#### C-CDA Sandbox Updates:
* None.

#### SITE V3.1.31| Released on: 11/22/2019

#### C-CDA Sandbox Updates:
* UI C-CDA Validator update to provide proper error when server is down.

#### ETT V2.3.18 | Released on: 11/18/2019
* Add filter to not permit a user to map the DCDT email addresses.

#### SITE V3.1.30| Released on: 09/30/2019

#### C-CDA Sandbox Updates:
* Fixed github vulnerabilities.
* Udated github link to new repository.
* Add support for vocabularyValidationConfigurationsErrorCount.
* Adds tracking for errors only in total vocabulary validations run.

#### FHIR Sandbox Updates:
* Added page title to client login and client registration pages.    

#### SITE V3.1.29 | Released on: 08/26/2019

#### C-CDA Sandbox Updates:
* None.

#### SITE V3.1.28 | Released on: 07/29/2019

#### C-CDA Sandbox Updates:
* Add severityLevel support to the C-CDA Validator UI
  * Adds the ability to select a severity level limitation for results returned. The user can now select the desired severity or severities. Selecting "Errors, Warnings, and Info" processes all available result types and is the default setting. The remaining selections limit the results as stated and should subsequently offer faster results".
* Support severityLevel limiting on the content validator in addition to prior support for the code validator and reference validator via the 'severityLevel' flag in a POST call.

#### FHIR Sandbox Updates:
* Added Provenance resource 
* Updated R4 to support additional search capabilities for Careplan, Condition, Devices, Encounter, Goal, Immunization, Medication Statement, Pediatric Weight For Height, Observation Lab, Smoking Status and BMI For Age resources. 
 * Bug fixes for DSTU2 and R4

#### ETT V2.3.15 | Released on: 7/29/2019
* Updated github links from siteadmin to onc-healthit - https://github.com/onc-healthit/reference-ccda-validator/releases/tag/1.0.42

#### SITE V3.1.27 | Released on: 06/24/2019

#### FHIR Sandbox Updates:
* Added delete client capabilities.
* Updated OpenID connect with introspection endpoint.

#### C-CDA Sandbox Updates:
* The C-CDA Validator now indirectly supports UTF files encoded with a BOM by removing the BOM before processing.
* The Reference C-CDA Validator API and static UI in local instantiations now support limiting MDHT Conformance and Vocabulary Validation results via their severity (Content limiting is coming soon). This has the potential to offer significant performance gains for users only interested in specific types of results, expecially on larger or issue-prone files. To use the feature, either use the static UI, or, send body form-data key:severityLevel and value:ERROR, WARNING, or INFO. Please note that selecting INFO will return all results, WARNING will return warnings and errors, and ERROR will return errors only.

#### ETT V2.3.14 | Released on: 6/24/2019
* https://github.com/siteadmin/site-content/blob/master/NewsAndAnnouncements.md
* Documentation and other updates to Dev and Test environments.

#### SITE V3.1.26 | Released on: 05/27/2019

#### FHIR Sandbox Updates:
* Updated EHR Launch Sequence Software to resolve defects when testing with Inferno by redirecting the launch correctly.
* Updated OpenID capabilities to pass Inferno testing.
* Fixed EHR Launch Sequence to pass Inferno testing.
* Updated Refresh Token sequence to return patient Ids.
* Updated Github with R4 Release.
* Updated FHIR Sandbox with test data to pass Inferno tests.

#### C-CDA Sandbox Updates:
* None.

#### SITE V3.1.25 | Released on: 04/29/2019

#### FHIR Sandbox Updates:
* Updated FHIR DSTU2 Server to allow Inferno to test SITE FHIR Server for Program Edition.
* Supported the Standalone Patient Launch Sequence.
* Added capabilities for EHR Launch Sequence.
* Fixed Password Reset capabilities.
* Added OpenID capabilities to the FHIR Server.

#### C-CDA Sandbox Updates:
* Updated C-CDA Configuration to fix Reference Validator Reboot issues on AHRQ Server.

#### ETT V2.3.11.1 | Released on: 03/28/2019
* 1. Add date header to MT tests 39, 40 and 41.

#### SITE V3.1.24 | Released on: 03/25/2019

#### C-CDA Validator Updates:
* A unit can now be equal to '1' in certain scenarios when it is selected from the UCUM value set. For local instantiations, the configuration is up to the user to apply with the new UnitAllowsOneValidator.
* CONF:1198-8559 was updated to enforce the if portion of the rule, "If Observation/value is a physical quantity (xsi:type="PQ"), the unit of measure SHALL be selected from ValueSet UnitsOfMeasureCaseSensitive (2.16.840.1.113883.1.11.12839) DYNAMIC
(CONF:1198-8555)."
* Updated doseQuantity/@Unit from the invalid value 'mg/actuat' to the valid UCUM value 'mg'.
* Updated value datatype in Result Observation (V3) from PQ to ST for 170.315_b1_toc_amb_ccd_r21_sample1_v12.xml and 170.315_b1_toc_amb_rn_r21_sample1_v12.xml. Note: due to this change, these file are now v13.
* The Reference C-CDA Validator and Code Validator API documentation material was updated to enhance the clarity for setting up local installations.

#### ETT V2.3.10 | Released on: 2/25/2019
* Updates to C-CDA validator library dependencies to use newer versions for compilers, jackson etc.
* Updates to C-CDA validator library dependencies to fix security vulnerabilities.
	
#### ETT V2.3.9 | Released on: 1/28/2019
* Update apache commons and apache tika version due to github identified security issue.
* Fix a bug in XDR HISP test cases where processed MDNs sent by the SUT cause inconsistent results.
* New validator release-https://github.com/siteadmin/reference-ccda-validator/releases/tag/1.0.38
	
#### ETT V2.3.8 | Released on: 11/26/2018
* Update jackson-databind version due to github identified security issue / Fix jackson dependency issues, upgrade both to 2.9.7.
* Implement a new RequiredNodeValidator for enforcing any missing node and add xpath support for the xsi namespace.
* Update configuration to resolve Lab test result with no units.
* Update configuration to resolve missing vocabulary rule for CONF:81-16850.

#### SITE V3.1.20 | Released on: 10/29/2018

#### C-CDA Validator Updates:
* Updated C-CDA Vocabulary Validator to match proper configuration paths and dynamic value sets where it was erroneous.
* Updated Test Data to remove external document reference from CarePlan.
* Updated Test Data to add R1.1 Template Id for Encounter Diagnosis to the DS4P Samples.

#### FHIR Sandbox:
* Updated DSTU2 Server to pass Inferno for Conformance Resources and for other specific clinical resources.

#### ETT V2.3.7 | Released on: 10/29/2018
* Updated internal libraries to better detect file mime types.
* Updated C-CDA Validator to handle NonUniqueResultException. Addresses google group user issues.

#### SITE V3.1.19 | Released on: 9/24/2018

#### FHIR Sandbox Updates:
* Updated FHIR sandbox with fixes to Bulk Data APIs.
* Added Inferno Testing Tool to SITE UI.

#### SITE V3.1.18 | Released on: 8/27/2018

#### C-CDA Validator Updates:
* Updated C-CDA Value Sets from VSAC to use the 6-15-2018 version instead of the older versions.
* Fixed Test Data to ensure no errors in samples based on the value set update.

#### ETT V2.3.5.1 | Released on: 08/27/2018
* Updated C-CDA Validator to use the 6-15-2018 value set release from VSAC.

#### ETT V2.3.5 | Released on: 08/16/2018
* IHE XDS Toolkit updated to the latest 6.3.4.
* More info in the SMTP MT tests fixed to reflect the appropriate email addresses.
* index.htm discrepancy (with respect to the inner ccda name) in the XDM (used by direct send) fixed.
* Internal mailbox adjusted to address the inbox overflow for the SMTP receive tests.

#### SITE V3.1.17 | Released on: 7/30/2018

#### C-CDA Validator Updates:
* Substance Reactant Value set was updated to the latest value set from VSAC.
* Added support for the latest LOINC.csv file to enable both 2015 baseline and newer versions of LOINC codesystem files.
* Updated VDT Test data XML file to remove errors from ERRATA update.

##### FHIR Sandbox Updates: 
* Updated FHIR Sandbox with Bulk API capability sample code and tutorials.

#### General SITE Updates:
* Updated SITE Contact Email to SITTeam@hhs.gov

#### ETT V2.3.4 | Released on: 07/19/2018
* XDR Test narrative updates to enhance user experience.
* The IMAP/POP inboxes updated to auto-populate test data from github periodically.
* Updated the XDM to address validation issues.
* Server security updates for better responsiveness.

#### SITE V3.1.16 | Released on: 6/25/2018

#### C-CDA Validator Updates:
* An invalid error no longer fires for recordTarget/PatientRole/Patient/Guardian when no code exists. The terminology portion of the error CONF:1198-5326 should only fire if the code exists and the terminology is invalid but was previously firing without a code.
* Added support for loading custom vocabulary configs in realtime.

#### ETT V2.3.3 | Released on: 06/25/2018
* Ability to select XDM zip option removed from the XDR (receive) cases to address the ambiguities arising from the metatdata in multiple locations. 
* The description in the D2 test for DCDT rendered accurate by changing it to "domain-bound".
* CCDA-validator updated. See release notes here: https://github.com/siteadmin/site-content/blob/master/CCDAValidatorReleaseNotes.md

#### SITE V3.1.15 | Released on: 5/29/2018

#### C-CDA Validator Updates:
* The validator has been updated to include the latest HL7 C-CDA Schema (with internal fix due to errata in HL7 Schema) which includes support for sdtc:functionCode in cda::Performer2 and cda::Participant2

#### C-CDA Scorecard / One-Click Scorecard Updates: 
* The scorecard has been updated to deduct points if the entire time element is padded to zero. For example: "19700501000000+0000" or "19700501000000-0000"

#### ETT V2.3.2 | Released on: 05/17/2018
* The direct endpoint - testing@ttpedge.sitenv.org augmented for both 1.1 and 2.1 validation based on the attachment.
* Server log architecture optimization.
* C-CDA validator updated to revert routeCode terminology and add routeCode/translation rule with terminology as per DSTU:1276 modification. 
* The modified implementation should look like the following:
  * <routeCode code="someValidCode" codeSystem="2.16.840.1.113883.3.26.1.1" codeSystemName="NCI Thesaurus">
  * <translation code="someValidCode" codeSystem="2.16.840.1.113883.6.96"/>
  * </routeCode>
* A single written example of the 4 locations modified is enforced as:
   * Immunization Activity (V3)
     1. MAY contain zero or one [0..1] routeCode, which SHALL be selected from ValueSet Medication Route FDA urn:oid:2.16.840.1.113883.3.88.12.3221.8.7 DYNAMIC (CONF:1198-8839).
     a.  The routeCode, if present, SHOULD contain zero or more [0..*] translation, which SHALL be selected from ValueSet Medication Route urn:oid:2.16.840.1.113762.1.4.1099.12 DYNAMIC (CONF:1198-32960).

#### ETT V2.3.1.2 | Released on: 05/01/2018
* Fixed ReactionObservation value set binding to Reaction Severity which was incorrect per HL7 clarifications received for ERRATA 836.
* Updated value set per ERRATA 1276 to reflect SNOMED-CT instead of FDA for routeCode.

#### SITE V3.1.14 | Released on: 4/30/2018

#### C-CDA Validator Updates:
* C-CDA Validator was updated to include HL7 approved September 2017 ERRATA for C-CDA R2.1. For more information please refer to https://groups.google.com/forum/#!topic/edge-test-tool/vsA_W9Yg4mc
* Test data was updated to make them conformant to the new ERRATA.
* Validator was updated to include document type validation for certification criteria.
* Validator was updated to allow resolved problems to appear as part of the Past Illness Section.
* The validator was updated to validate document type and indicate errors based on the certification criteria, previously this was being done visually by the ATLs.
* The validator was updated to allow resolved problems to appear as part of the History of Past Illness section.
* The Test XML files for CIRI for R11 version was updated to properly link narrative with entries.

#### ETT V2.3.1.1 | Released on: 4/30/2018
  * ETT updated with enhanced database security measures.

#### ETT V2.3.1 | Released on: 4/19/2018 
* XDR Test 2 enhanced so that ccda document type can be specified and received document validated accordingly.
* Database security enhanced with encryption measures.

#### SITE V3.1.13 | Released on: 3/26/2018

#### C-CDA Validator Updates:
* C-CDA Validator was updated to remove Encounter Diagnosis validation errors from View, Download, Transmit criteria.
* Updated RelationshipType value set for CarePlan documents.

#### FHIR Sandbox updates:
* Updated Google Analytics for FHIR Sandbox
* Updated Bulk FHIR API Server and deployed Beta Version.

#### ETT V2.3 | Released on: 3/15/2018 
* R2.1 validator UI now includes download files option.
* C32 and CCR files removed from Send Direct Message and Documentation.
* Mime headers removed from the downloaded ccda file sent using direct.
* Test data update: Modified test data for Care Plan (b)(9) criteria to identify clearly the optionality and required data for Care Plan sections

#### SITE V3.1.12 | Released on: 2/26/2018

#### C-CDA Validator Updates:
* C-CDA Validator was updated to produce warnings for care plan sections that are mentioned in the test data but are a SHOULD in the IG.
* Updated IG validation to align MedicationSection/code rules with R1.1 C-CDATemplateLibrary.

#### C-CDA Scorecard / One-Click Scorecard Updates: 
* Modify lowScoringSample from R2.0 to R1.1
* Multiple 508-compliance updates to the PDFs
* Add author, subject, keywords, and language metadata for 508
* Update Conf and Cert links to full text vs count only for 508
* Update top 2000 LOINC codes link in UI report for 508
* Fix Back to Top links for 508
* Make submitted email address a link as per 508
* Add scoping to dynamic table as per 508 5.9

#### ETT V2.2 | Released on: 2/15/2018 
* C-CDA Validator UI has been revised - addition of validator home page, IG only option for 2.1
* Bookmark attribute changed to "ETT Home".
* HISP SMTP Test 8, 14, 'More Info' updated.
* R2.1 validator flips the report after the validate button is selected.
* Test by criteria/Surveillance reorganized to include : (b)(1), Criteria (I)(A) Send using Edge Protocol - Delivery Notification
* Heading and test panel in the Surveillance test for Direct has been updated 
* Enhanced google analytics.
* SMTP Test 28 message subject typographic error has been fixed 

#### SITE V3.1.11 | Released on: 1/29/2018

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Add button with link to ONC One Click Scorecard page
* Added ccdaVersion and service errors for invalid formats

##### C-CDA Validator Updates: 
* Added ccda file name of the submitted file for debugging.
* Added warning messages for telecom content validation.

#### ETT V2.1.2.3 | Released on: 1/29/2018
* Added ccda file name of the submitted file for debugging. 
* Added warning messages for telecom content validation.
* Updated MU Gold Sample XML file to remove Clindamycin Allergy which is not present in the test data.
* Updated CIRI R1 xml samples files to correct medication dosage.
* Updated CarePlan PDF's to explicitly mention the Medication Tylenol for the Intervention Act referring to the Medication Entry.

#### ETT V2.1.2.2 | Released on: 12/14/2017
* Enabled AUTH LOGIN support for the SMTP send/receive tests (in addition to the earlier supported AUTH PLAIN for Plain SASL authentication mechanism).

#### SITE V3.1.10 | Released on: 11/30/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Collects and returns service errors from the referenceccdavalidator/Ensures files with service errors can never show invalid results
* Regenerated all Try Me samples which fixes issues with downloaded Try Me matching generated results
* Added Google Analytics to various Scorecard events
* Updated One Click report to track industry Average per specific C-CDA document type (CCD, DS, RN, CP, etc.)
* Store Direct Address in the DB for One Click Scorecard
* Improved performance with multithreading

##### C-CDA Validator Updates: 
* The C-CDA Validator was updated to 1.0.25 with the following fixes.
* The C-CDA validator was updated to allow for Translation element within the raceCode attribute to be used to represent granular race code.
* The C-CDA Validator was also update to fix the vocabulary defect which prevented validation in certain cases with the error message "The service has encountered the following error: result returns more than one."

##### FHIR Sandbox Updates: 
* Updated the FHIR Deployment to support TLS1.0

#### ETT V2.1.2.1 | Released on: 11/30/2017
* Updated Direct LDAP Certificate Discovery to account for userCertificate:binary attribute which is used to store direct certificates in certain systems. Prior to this fix the certificate associated with a Direct address stored in the attribute "userCertificate:binary" was not being discovered successfully where as certificate stored in "userCertificate" was being discoverd.
* Updated the C-CDA Validator to 1.0.25 version which can be accessed at - https://github.com/onc-healthit/reference-ccda-validator/releases
* The C-CDA validator was updated to allow for Translation element within the raceCode attribute to be used to represent granular race code. 
* The C-CDA Validator was also update to fix the vocabulary defect which prevented validation in certain cases with the error message "The service has encountered the following error: result returns more than one."
* Updated the 170.315(b)(2) CIRI Sample XML files with the right Diagnosis code of 282291009 instead of the incorrect code (29308) which is currently present.

#### ETT V2.1.2 | Released on: 11/16/2017
* Updated Test Descriptions for XDR MT Test 50a and 50b to move the email addresses to the “More Info” screen.
* Updated the “More Info” screen for SMTP Test 26a and 26b to document the expected outcome.
* Added a link to the documents and help from ETT Home page.
* Removed Email addresses for various MDN endpoints from ETT HISP and Edge Home pages since the addresses are already part of the Test Cases.
* Removed 2015 Edition Direct Content Validation endpoints from ETT HISP and Edge Home.
* Clarified “Vendor Email Address” as “Vendor Direct Email Address” as part of the ETT UI.
* Added a link to the FAQs as part of the Documents page.
* Corrected Typos in XDR Tests 10, 11 and 12 on More Info pages.

#### SITE V3.1.9 | Released on: 10/30/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected One Click Scorecard Report Schema errors report.
* Added total number of C-CDA scored so far for average calculation.
* Added API to get Scorecard Metrics downloaded.
* Added fix for missing document type in C-CDA Scorecard Metrics database.

##### C-CDA Validator Updates: 
* The C-CDA Validator was updated to 1.0.24 with the following fixes.
* The latest value sets from VSAC were installed and configured as part of the release.
* Removed the Console Logger to prevent large log files.
* Fixed the Address Zip Code Value Set validation.

##### FHIR Sandbox Updates: 
* Updated the FHIR Resources with fixes based on validation reports produced by FHIR profile validator.

#### ETT V2.1.1.1 | Released on: 10/30/2017
* The C-CDA validator has been updated to Release 1.0.24 which can be accessed here: 
    - https://github.com/onc-healthit/reference-ccda-validator/releases
* As part of the release, the latest Value Sets from VSAC have been downloaded and configured.    
* For more information about the Value Sets, please refer to the github location - https://github.com/onc-healthit/code-validator-api/tree/master/codevalidator-api/docs
* The Code Validation has been updated to print warnings for inactive codes as specified by the CodeSystem files.

#### ETT V2.1.1 | Released on: 10/19/2017
* Adding Direct address to Direct Home page - To verify basic Direct send capabilities of your system send a message to:testing@ttpedge.sitenv.org.
* Updated Direct Home Page with more enhancements.
* Removed orphan listing in the Surveillance (h)(2) dropdown array
* Corrected SMTP MT Test 46 to display the correct test status - distinctly showing "Failed" instead of the generic "Retry" in case of messages without the header.
* Updated the files in the inboxes for POP & IMAP Test 31 with the current versions.
* Changed Text in XDR MT Test 13, 14, 16
* Fixed SMTP Receive Tests 29 and 29 contain two METADATA.XML files
* Fixed - CCDA Validation Report link doesn't work for (h)(2) SMTP Send 8, 14 and (b)(1) SMTP Send 8, 14, 18
* Fixed the ttpds2 DNS MX entry to return the host name instead of IP
* nodeRepresentation attribute missing for author in XDR tests 3/5 - fixed and verified.
* Collecting usage analytics for various user functions.

#### ETT V2.1.0.2 | Released on: 9/27/2017
* 2015 Edition Testing by Criteria 
  * lists duplicate entries in the criteria dropdown - fixed.

#### SITE V3.1.8 | Released on: 9/26/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected One Click Scorecard Report Schema errors display to use proper sentence.

##### C-CDA Validator Updates: 
* The C-CDA Validator was updated to 1.0.23 with the following fixes.
* Updated the 170.315(b)(2) - CIRI Validation for R1.1 files which was missing. Prior to the release, the R1.1 file reconciliation output submitted to the validator was not being validated for content. This was updated to ensure content matching was performed with the R1.1 reconciliation file outputs. So if the reconciliation of R1.1 files does not produce the output following the instructions provided for the criteria, there will be errors displayed by the validator.
* Existing Smoking status validation bug was fixed which was previously preventing an error being displayed when smoking status entry was nullFlavored or missing. The fixing of the bug displays an error if smoking status does not include the proper test data provided.
* DS4P Validation was updated such that PurposeOfUseSecurityObservation/value and all other values and codes of templates which inherit from SecurityObservation now override their parent requirements. This allows for both templates to exist, but only the child's requirement to be enforced. This resolves the possible conflict of differing terminology requirements between a parent and child template. As a result, PurposeOfUseSecurityObservation value/@codesystem now requires ActReason 2.16.840.1.113883.5.8 as opposed to the prior requirement of ObservationValue 2.16.840.1.113883.5.1063, due to an error in the HL7 example XML.

#### ETT V2.1.0.1 | Released on: 9/25/2017
* Direct 
  * The endpoint dsn@ttpedge.sitenv.org which was unused as part of ETT tool and 2014 and 2015 Test procedures was removed as it was causing exchanging unnecessary messages with HISPs who sent messages to the endpoint in a continuous loop causing a lot of unnecessary network traffic.
* C-CDA Validator: The C-CDA Validator was updated to 1.0.23 with the following fixes.
  * Updated the 170.315(b)(2) - CIRI Validation for R1.1 files which was missing. Prior to the release, the R1.1 file reconciliation output submitted to the validator was not being validated for content. This was updated to ensure content matching was performed with the R1.1 reconciliation file outputs. So if the reconciliation of R1.1 files does not produce the output following the instructions provided for the criteria, there will be errors displayed by the validator.
  * Existing Smoking status validation bug was fixed which was previously preventing an error being displayed when smoking status entry was nullFlavored or missing. The fixing of the bug displays an error if smoking status does not include the proper test data provided. 
  * DS4P Validation was updated such that PurposeOfUseSecurityObservation/value and all other values and codes of templates which inherit from SecurityObservation now override their parent requirements. This allows for both templates to exist, but only the child's requirement to be enforced. This resolves the possible conflict of differing terminology requirements between a parent and child template. As a result, PurposeOfUseSecurityObservation value/@codesystem now req
* Test Data Updates:
  * The R11 Receiver files (XML files) for 170.315(b)(1) and (b)(5) were updated to correct the telephone numbers to be consistent between the narrative display content and the coded information.
  * The Negative Testing Files for CCDS (Both R2.1 and R1.1) were updated to remove “Bad/Fictitious” template Ids , since vendors were interpreting these templates as open templates and hence not flagging the errors. The omission of these templates and corresponding entries with the right template Ids will make the test data less confusing, so that vendors can directly identify which templates are missing and erroneous based on the C-CDA IG.
  * The DS4P Sample 1 files were updated based on the DS4P issues resolved in the validator above.

##### FHIR Sandbox Updates: 
* Updated and fixed DSTU2 and STU3 validation for FHIR Tools.
* Fixed OAuth issues incluing password encryption, state parameter validation, removing cached authorization.

##### Direct Transport Sandbox Updates: 
* Added capability of using Interop@direct.hhs.gov for Direct Trust Users 

#### ETT V2.1 | Released on: 9/21/2017
* "Surveillance Testing" aspect added to ETT - accessible from the ETT home page.
* DCDT Trust Anchor download option fixed.
* Added help (hover) descriptions to the Direct Certificates
* Send Direct Message issue - adding hash value to the file extension - has been fixed. 

#### ETT V2.0.1.2 | Released on: 9/15/2017
* The release updates the Direct Certificates related to the domains 
  * ttpedge.sitenv.org 
  * ttpds2.sitenv.org
* The certificates are being updated to remove the invalid CRL URI in the certificates. These certificates will be published via - DNS and will propagate shortly after the release is done.
* Note: The trust anchors or intermediate anchors are not being updated, so vendors do not need to change any trust anchors. 
* The Direct transactions should pick up the new CERTS that get published via DNS after the release.

#### SITE V3.1.7 | Released on: 8/29/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected Rubrics for Timestamp handling of Problems and Allergy Concern acts
* Corrected Rubrics for Narrative Text linking.
* Posted Rubrics document to the Website.

##### C-CDA Validator Updates: 
* Fixed DS4P validation to align with the DS4P IG and the Consent Directive IG.
* Fixed CCDS Content Validation for UDIs

#### ETT V2.0.1.1 | Released on: 8/28/2017
* Issue with XDM Validation Report download fix for application/octect-stream corrected.
* Register Direct Title has been updated.
* Updated C-CDA Validator with the following fixes
  * Fixed DS4P validation to align with DS4P IG and Consent Directive IG as they are dependent.
  * Resolved errors in test data samples provided by ONC.
  * Updated Code Validator to handle the new VSAC format.
  * Updated the test data to contain the previous version also.

##### FHIR Sandbox Updates: 
* Updated and fixed DSTU2 validation loging for DSTU2 FHIR Sandbox.

#### ETT V2.0.1 | Released on: 8/17/2017
* Send Direct Message - help hover text for "Wrapped" selection enhanced.
* Register Direct narrative has been updated.
* Security settings in the server improved
* XDM Validation Report download fixed: now accepts application/octect-stream.
* The following C-CDA updates have been made as part of the release and will be visible from Friday (8/18/2017) evening.
    * Removed non-CCDS data elements from (g)(9).
    * Updated Immunization test data in PDF files to remove inactive codes.
    * Updated Medication test data in PDF files to remove inactive codes. 
    * Updated XML samples to remove non-UTF8 characters and inactive codes.

#### SITE V3.1.6 | Released on: 8/1/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected issues with Date of Death Rubric timestamp validation.
* Added Rubric for Substance Administration Sig validation.
* Corrected issues with data encoding and handling UTF-8.

##### C-CDA Validator Updates: 
* Fixed DS4P validation to kick in correctly based on objectives.
* Updated Reference Validator to use 20170725 MDHT build and 20170707 DS4P build
* Updated Encounter Diagnosis content validation to conform to test data.
* ETT
  * Fixed Parsing errors in XDR Test 1 and 3.
  * Fixed intermittent database exception error while executing XDR Test 1.
  * Updated Mime Types for SMTP 26a and 26b
  * Updated Attachment Processing for XDR Test 1 to handle HTML and XML attachments sent together.
  * Fixed XDM Validation Report download capability.
  * Updated Cronjobs to populate mailboxes used by SUTs.

##### FHIR Sandbox Updates: 
* Fixed error handling of Queries.
* Made text changes to remove Alpha Release, Run US Core Tests, Public client, Confidential client.
* Added Validation for STU3 Server in FHIR Query Tool.
* Added initial validation for DSTU2 Server responses in FHIR Query Tool.
* Updated data to trim white spaces for various FHIR data elements.

#### ETT V2.0 | Released on: 07/20/2017
* ETT has been updated with a new look and feel consistent with the rest of the ONC suite of applications.
* The timeout used in XDR MT 44 is now configurable for more effective testing.
* Direct Messages sent now have "Test Session Name" added to the Subject header
* (SMTP test 8, 14) and (SMTP Test 8, 14, 18) descriptions have been updated.
* HISP XDR Test 17 adds "https://" to the description.
* Failure MDN returned from ETT now has the disposition value 'failed' as per the IG
* Validation is performed only if C-CDA in XDR and XDM sender tests.
* XDR MT tests have improved documentation on endpoints used - particularly XDR MT Tests 43/44/50a/50b.

#### ETT V1.2.6.1 | Released on: 6/27/2017
* XDR MT 43/44 issue resolved. ETT sends a failure MDN to the SUT HISP as per the test specification without time delay; for 44 however it maintains the delay and the description has been updated to document the delay.
* XDR 7 displays the https endpoint correctly now for copying from clipboard to be used for the test by SUT.
* ETT refreshes IMAP/POP account folders more frequently so that testers will not be affected by occasional problems with missing mails.
* CCDA-validator has been released. The release notes here:
  * Updated typeCode identification in ConsultationNote2 participant which was causing errors incorrectly.
  * Updated Problem Value Set from VSAC to accomodate Allergy Reaction codes.
  * Updated Content Validation to not have an error when the Severity has a nullFlavor value.
  * Updated Content Validation to produce WARNING instead of ERRORS when Allergy Reaction and Severity are not present or are present with Null Flavors.
  * Updated Content Validation to allow Lab Result Values without Units to use either PQ or ST data type.
  * Updated Content Validation to fix defect in PQ validation which was preventing errors when just value was not matching the test data.

#### SITE V3.1.5 | Released on: 6/26/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected issues with Date of Birth Rubric timestamp validation.
* Corrected defects with lifespan validation rubric when observations occured at the same time as patient's death.
* Added rubric for Birth Sex Validation.
* Added rubric for Patient's Alternative Name Validation.
* Updated Metrics collection APIs to segregate One-Click Scorecard and UI.
* Updated Metrics to collect section based scoring, document based scoring.
* Changed Error Sample of Scorecard to get a C instead of A-.
* Updated HL7 Templates to include DS4P Templates.
* ETT to 1.2.6.1
  * XDR MT 43/44 issue resolved. ETT sends a failure MDN to the SUT HISP as per the test specification without time delay; for 44 however it maintains the delay and the description has been updated to document the delay.
  * XDR 7 displays the https endpoint correctly now for copying from clipboard to be used for the test by SUT.
  * ETT refreshes IMAP/POP account folders more frequently so that testers will not be affected by occasional problems with missing mails.

##### C-CDA Validator Updates: 
* Updated typeCode identification in ConsultationNote2 participant which was causing errors incorrectly.
* Updated Problem Value Set from VSAC to accomodate Allergy Reaction codes.
* Updated Content Validation to not have an error when the Severity has a nullFlavor value.
* Updated Content Validation to produce WARNING instead of ERRORS when Allergy Reaction and Severity are not present or are present with Null Flavors.
* Updated Content Validation to allow Lab Result Values without Units to use either PQ or ST data type.
* Updated Content Validation to fix defect in PQ validation which was preventing errors when just value was not matching the test data.

##### FHIR Sandbox Updates: 
* Initial Release of FHIR Scopes checking.
* Added ability for FHIR Query Tool to call Secure FHIR Server.  

##### SITE UI: 
* Updated Broken Link to NIST ETT to point to ONC ETT.

#### ETT V1.2.6 | Released on: 6/15/2017
* Restore tests for the 2014 Edition to the UI
* Remove IMAP/POP 12 tests
* DCDT issue fixed whereby test case selection is prompted after reset
* Content-Disposition check in the direct validation  enhanced to allow paranthesis inside quotes
* Fixed: Message Validators showing Criteria instead of C-CDA Document Type

#### SITE V3.1.4 | Released on: 6/1/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* The C-CDA Scorecard was updated with the following changes:
  * Removed industry averages from the Scorecard Report generated by the SITE UI.
  * Added One-Click Scorecard links to Direct and C-CDA Sandboxes.

##### FHIR Sandbox Updates: 
* Supported DSTU2 and STU3 resources according to US Core Implementation Guide.
* Added missing queries to DSTU2 and STU3 Servers. 

##### C-CDA Validator Updates: 
* Fixed Immunization Value Set in MDHT.
* Accepted Code Modifications from the community for Code-Validator.
* Changed 2015 Certification Test Data to accomplish the following
  * Made Document Ids across all the samples to make them unique.
  * Updated RxNorm Codes in R11 Samples to use prescribable drugs.
  * Updated Care Plan documents to include US Realm Header and R11 Section/Entry Template Ids.
  * Fixed Language Code for Care Plan Samples.

#### ETT V1.2.5.1 | Released on: 5/31/2017
* The C-CDA Validator was updated to Release 1.0.17 and it can be accessed here : https://github.com/onc-healthit/referenceccdavalidator/releases
* Select by Criteria b(1) issues have been corrected.
* Miscellaneous documents links to 2014 certification samples from github. 

#### ETT V1.2.5 | Released on: 5/18/2017
* IMAP/POP folders populated periodically.
* UI updataes: More info XDR Test 1, MT Test 20a/b, Rename HISP IMAP/POP Tests, Update Test by Criteria drop-dwon labels (h)(2),
   Labels for IMAP/POP 31, XDR 3 address corrected, SMTP Test 1 text changed to "non-existent address", DCDT accordian hyperlink at the top fix.
* XDMs used in the tests changed to uppercase.
* Content Disposition check ignores comment check for quoted strings for Direct Message Validation.

#### ETT V1.2.4.3 | Released on: 5/09/2017
* Fixes the issue with attachments in the b(1) due to encoding

#### SITE V3.1.3.1 | Released on: 5/8/2017

##### C-CDA Scorecard Updates: 
* The C-CDA Scorecard was updated with the following changes:
  * Fixed defects related to display name validation for code systems that do not exist in the vocabulary database.
  * Fixed effective time handling related to patient lifespan when there is a nullFlavor for any of the times being compared. 
  * Fixed effective time handling when there are just a single timestamp value vs a low and high for comparison with other time intervals.

##### FHIR Sandbox Updates: 
* Corrected defects which was preventing the Observation related profiles from returning data.
* Corrected defects to remove scopes from open server screens.
* Added additional missing US Core profiles in the Query Tool.

#### ETT V1.2.4.2 | Released on: 4/28/2017
* Fixes the issue with the XDR tests adding extraneous "http" in the endpoint.

#### SITE V3.1.3 | Released on: 4/25/2017

##### C-CDA Validator Updates: 
* The C-CDA validator was updated with the following changes:
  * Fixed defects related to the Content Validation for Care Plan criteria (b)(9), CIRI criteria (b)(2) and DS4P criteria (b)(7).
  * The defects were not validating the patient names correctly, the data in the document sections as needed for the criteria.

##### FHIR Sandbox Updates: 
* Updated FHIR Sandbox with to support STU3 server.
* Updated FHIR Sandbox to add validation service for future integration with conformance tool.

#### ETT V1.2.4.1 | Released on: 4/25/2017
* The Direct Certificate Discovery Tool has been updated to use the ETT UI framework.
* As a result, the new links to the tool are :
  * 2014 DCDT: https://ttpedge.sitenv.org/ttp/#/direct/certdiscovery/dcdt1
  * 2015 DCDT: https://ttpedge.sitenv.org/ttp/#/direct/certdiscovery/dcdt2
* The old links will not be accessible going forward.
* The C-CDA Validator was updated to Release 1.0.16 and it can be accessed here :    
  * https://github.com/onc-healthit/referenceccdavalidator/releases

#### ETT V1.2.4 | Released on: 4/20/2017
* Added option to selectively use STARTTLS (default selected) for SMTP/IMAP/POP profiles for systems demonstrating security through other means such as secure networks.
* Testing by Criteria § 170.315(b)(1) updated for accuracy.
* Content type for SMTP 25d order updated to reflect the correct types.
* UI fixes:  timeout field in SMTP MT 28 removed, endpoint listed for XDR Test 7 fixed,  removed *: from the XDR MT Direct From Address hover over

#### SITE V3.1.2 | Released on: 3/28/2017

##### C-CDA Validator Updates: 

* The C-CDA validator was updated with the following changes:
  * Update to the latest code validator API that fixes a bug with loading SNOMED display names.
  * Update to the latest MDHT build which merges R11 and R21 validation.
  * Relaxed ERRATA #596 for R11 from an ERROR to a WARNING.
  * Updated to the latest content validator API to accomodate Procedure Activity Acts as entries for Procedure content validation.

##### C-CDA Scorecard Updates: 
* Update the 'Low scoring sample' in the 'Try Me' to a sample with more issues
* Remove 'Beta' header to align with the 1.0 release
* Implement system to force browser to always load the latest release for new deployments
* Add error count per category to save report/UI-based PDF
* Sort PDF Categories by score, null, certifcation, and IG results as a form of severity
* Update to use TTP endpoints for referenceccdavalidator calls
* Expand and improve source code testing, performance, and configuration
* Defect Fixes
  * Remove 'Detailed Results' header in saved PDF if there are no results
  * Fix code system check for Null Pointer Exception.

##### FHIR Sandbox Updates: 
* Updated FHIR Sandbox with Medication Data Set from ONC MedList project.
* Updated FHIR Server Capabiltiy Statement (Conformance Statement) for STU2 version.
* Updated FHIR Server to support all Argonaut queries.

##### SITE UI Improvements:
* XDR Test Tool updated with the new UI themes, headers and footers.

#### ETT V1.2.3.1 | Released on: 3/27/2017
* CCDA validator (2.1 and 1.1) updated to 1.0.5.  Release notes can be accessed here : https://github.com/onc-healthit/referenceccdavalidator/releases
* The criteria (b)(1)(i)(C) XDM Processing was wrongly listed as (i)(B) in the dropdown - fixed.

#### ETT V1.2.3 | Released on: 3/16/2017
* "Test By Criteria" - (b)(1)  has been added for easier navigation for this criteria.
* Updated test by criteria h(2) to include "Send using Direct + XDM".
* h(1) (ii) criteria now adds upload file button for uploading certificates.
* The direct validation link issue due to un-encoded url is now fixed.
* SMTP 18(a)/47(a) deliver the MDNs from ETT to the user specified address, though still needs to be validated manually (see: https://groups.google.com/forum/#!msg/edge-test-tool/S-QqSkxTzRE/tTfocNK2CQAJ)
* All the SMTP receiver tests now have the manual validation workflow
* SMTP MT 28 allows configuration for timeout value 
* More info sections have been updated for Edge IMAP, Edge POP, XDR 10/11/12, SMTP 18, Direct From/Direct To for XDR tests
* UI fixes: documents page links shown with right icons, read version numbers from github
* The ccda-validator has been updated with these changes :
  * Updated the Negative Test XML Files for (b)(9) Care Plan criteria to include the US Realm Header Template Id.
  * Update the Administrative Gender value set to include the "UN" code.

#### SITE V3.1.1 | Released on: 2/28/2017

##### C-CDA Validator Updates: 

* The 2015 Edition C-CDA Validator has been updated to Release 1.0.14 with the following changes.
  * Relaxed the Birth Sex validation to be a WARNING instead of an ERROR when it is missing in the Social History Section.
  * Relaxed the Previous Name validation to be a WARNING instead of an ERROR when the HL7 recommendation is not used to code a previous name.
  * Fixed the Reference C-CDA Validation to handle case sensitivity on Language Code. 
  * Fixed Patient Suffix validation to account for punctuations.
  * The C-CDA Validator Instances between SITE and ETT have been consolidated to have a single instance.
  * Updated the SITE C-CDA validator to use the ETT C-CDA validator.

##### C-CDA Scorecard Updates: 
* Updated the scorecard to use the ETT C-CDA Validator.

##### SITE UI Improvements:
* Direct Sandbox changes to remove unused tools.
* Direct Sandbox changed to only contain the Direct Test Tool and XDR Test Tools.
* FHIR Sandbox Header/Footer Updates.

##### FHIR Sandbox Updates: 
* Updated DAF-Core to US-Core
* Updates to add Medication Data to Resources based on ONC Med List project.
* Updates to support US-Core Queries in the FHIR Server.

##### DCDT Updates:
* Updated DCDT to address mixed case issues. 
* Updated DCDT to host anchors on port 80.


#### SITE V3.1.2.2.1 | Released on: 2/28/2017
* C-CDA Validator Updated to version [1.0.14](https://github.com/onc-healthit/referenceccdavalidator/releases/tag/1.0.14)

##### C-CDA Validator Updates:

* The 2015 Edition C-CDA Validator has been updated to Release 1.0.12 with the following changes. 
  * CPT vocabulary validation has been added and Procedure entries can use CPT codes as part of their structured data. 
  * Updated Display Name validation API used by the scorecard.

##### SITE UI Improvements:

* C-CDA R1 validator now shows error messages returned from the service
* Improved UI for small-screen devices where possible
* System messages will display under the banner when the SITESystemMessage markdown has content. ( https://github.com/onc-healthit/SITE-Content/blob/master/SITESystemMessage.md )
* Upgraded to Angular 2.4.7
* Build using AOT flag that uses ahead-of-time JavaScript compilation (new feature of Angular CLI BETA-31)
* Installed and configured Google’s PageSpeed Module for Apache ( https://developers.google.com/speed/pagespeed/module/ )
* Fixed sitenv.org Apache config to always forward to HTTPS

##### Scorecard Updates:

* The Scorecard was updated with the following changes 
  * The One-Click Scorecard for HIMSS 2017 was configured.
  * The PDF Report was updated to have a summary and a interpretation guide.
  * The Scorecard Display Name Validation was updated to leverage all the possible names in the vocabulary.
  * The Conformance Errors were seperated from Certification Feedback.
  * Updated Effective Time Element handling of partial times.
  * Updated scoring logic to account for missing sections.
  * Updated scoring rule for Lab Result validation and Vital Signs validation to look for PQ data type and enforce UCUM rules.
  * Updated scoring rule for top 2000 LOINC codes. 
  * The detailed Scorecard release notes can be accessed at ( https://github.com/onc-healthit/SITE-Content/blob/master/CCDAScorecardReleaseNotes.md ) 

##### ETT V1.2.2 | Released on: 2/16/2017
* "Test By Criteria" - h(2) has been added for easier navigation for this criteria.
*  SMTP HISP MT tests for SMTP receiver 1-4, 21(a), 23(a), 24(a), 25(a), 26(a), 27(a), 28(a), 29(a) and Edge MT tests 18(a), 47(a) incorporate the workflow for manual verification of the MDN.
*  XDS Toolkit updated - which in particular addresses, [XDR validation of sourcePatientInfo does not permit PID-3 identifier list](https://github.com/usnistgov/iheos-toolkit2/issues/193)
*  Test Data XDM_LIM.zip updated - details [here](https://groups.google.com/d/msgid/edge-test-tool/cfc85156-c6d5-447e-96a4-170f2c895911%40googlegroups.com)
*  SMTP HISP Test 1-8, 14 (Send) Test - endpoint changed to edge-receiver@ttpds.sitenv.org to enable local delivery (AUTH not required).
*  SMTP MT 45 Description updated.
*  UI changes: Certificate upload text for SMTP MT Tests now indicates that a .der file is required., download page shows external links.


#### SITE V3.1.0 | Released on: 1/31/2017

##### C-CDA Validator Updates:

* The 2015 Edition C-CDA Validator has been updated to Release 1.0.11 with the following changes. 
  * Substance Reactant value set for Allergies has been updated to contain the full list of values. (Previously it was a partial list)
  * Improved performance of the vocabulary validation.
  * Updated underlying MDHT JAR files to support R1.1, R2.1, DS4P and other related validation in a single WAR file.
  * Also the updated MDHT JAR files have performance and multi-threading improvements.

##### C-CDA Test Data Updates:
[Test Data Update Details](https://groups.google.com/forum/#!topic/edge-test-tool/EK91BXBhLSY)

##### SITE UI Improvements:

* Updated the Direct Transport Sandbox to use the new UI style and themes.
* Removed Liferay Portlet infrastructure for Direct Sandbox and created new services for existing capabilities.
* Added Breadcrumb navigation to the UI.
* Changed NIST Tools page to Test Tools.

##### Scorecard Updates:

###### Improvements
* Updated Effective Date Time Rule to handle partial dates/times
* Updated Unique Id rule to not apply on the header participants such as Author
* Updated Display Name rule to not apply when display names are not present
* Updated Text Reference Checking Rule to account for sub elements in tables in the narrative text
* Updated Scoring criteria to not apply rules to No Information or Null Sections which have no data or are completely absent
* Updated Try Me to support multiple files (a high and low scoring sample and a sample with errors) and provided new and updated data
* Updated top level results and summary UI layout
* Added ability to identify 2015 Edition Certification Feedback and Empty Sections in the heatmap
* For clarity, converted rubric sub-Description data ('Issues' and 'Best Practice') into tabs versus links
* Embolden heat map text by default and hover attributes so that categories are both easier to read upfront and understand the status of overall
* Added disabled option to the heatmap when categories have no issues to navigate to or are empty sections
* Updated Conformance and Certification section to display a related issue count in brackets
* Updated heatmap to jump to Certification or Conformance when a section has related issues versus jumping to a no-issue scorecard result
* Categories (including Conformance and Certification) which have no issues are no longer shown in the detailed results which allows for a cleaner, more focused interface
* Updated IG/Cert. links to navigate via their label versus error count alone
* Added C-CDA Document Type (e.g. CCD) scored
* Each rubrics 'Issues' tab is now selected/expanded by default
* Replaced loading text with animations
* Reworded and moved 'Standard' option text to the end of each rubrics description versus in its own tab
* Updated to not load 'Detailed Results' button on a full pass scenario (100/100)
* Added 'Edition' to 2015 Certification Feedback
* Updated color schemes
  * 3 colors only (green, yellow, red) for all grade results
  * Category headers black versus blue to match heatmap
  * Cert and IG black in heatmap and detailed results
  
###### Fixes
* Fixed heatmap category click/IG and Cert. links not opening detailed results if closed
* Fixed issue where a C-CDA IG Conformance Error could be identified as a 2015 Edition Certification Feedback issue in the heatmap
* Fixed typos in a few locations

#### ETT V1.2.1 | Released on: 1/19/2017
* Select by criteria 170.315(h)(1) now lists all the steps needed for the test
* The file dialog selection of ccda-documents are mandatory for all the cases except the SMTP MT 39/40/41.
* Descriptions on EDGE MT - SMTP MT Tests 18a and 47a updated.
* Included XDS Toolkit 4.2 (allows multiple patient IDs within a sourcePatientInfo)
* UI changes: all the footers now consistent, profile user input is also consistent, added copy "widget" to the CCDA R2.1 Direct (to) address section, XDR validation changed from "NOSAML" to "No SAML", XDR "Link to Certificates" to "Click to download XDR TLS certificates".
* Documentation updates: User Manual inclues the section "Test By Criteria", Local installation guide and installing from       AMI guide  included in the github and as a link from the Documents page.
* Updated the XDM_LIM.zip in the github testdata which fixes a validation issue with the slot (used by XDR MT 11).
* Update: 1/31/2017 -  Updated the XDM_LIM.zip/XDM_FULL.zip - https://groups.google.com/forum/?utm_medium=email&utm_source=footer#!msg/edge-test-tool/YrgbgRix5vo/e6FZQukhDAAJ

##### ETT V1.2.0.1 | Released on: 12/23/2016
* Fix broken URL calls.

#### SITE V3.0 | Released on: 12/20/2016

* Updated CCDA Validator with the following fixes
  * Relaxed the timing information validation for Problems, Medications, Allergies.
* Updated new MDHT Release which includes the following ERRATA for C-CDA R2.1 (710, 806, 808, 872, 986, 1018, 1220)
* Scorecard fixes and enhancements
  * Added the ability to score multiple C-CDA files
  * toggle IG Conformance/Certification results
  * improved proecessing time
* New SITE UI released
* Updated FHIR Sandbox with bug fixes idenified by ONC Testing.

##### ETT V1.2.0 | Released on: 12/19/2016
* New panel to the ETT Home page "Test By Criteria" has been added - allowing logical navigation of the test cases. This release addresses a part of criteria § 170.315(h)(1) and the remaining criteria to be addressed in the upcoming releases.
* Certificate discovery in ETT (for Direct Send) now uses the certificate that has not expired if multiple certificates are encountered.
* ETT now adds the Disposition-Notification-To header in the Message Tracking HISP cases.
* XDR Validator - Turning SAML off now shows "No SAML" instead of "No Errors" in the SAML tab.
* The tool has been fixed to skip malformed or corrupted messages in the ETT mailstore folder which cause issues when fetching emails.
* Documentation updates:
  * Added link to FAQ in the Help Page
  * Hosting Training Videos on ETT again - please note that the references to nist.goSITE Vserver names in the videos need to modified accordingly (to sitenv.org equivalent).
  * Removed Section 3, Local Install from the User Guide. This will be included in the Installation Guide.
  * CCR/C32 samples from the documents page are now linked to the github repository.	  
* UI changes: Tool tip indicator for 'Message format' on File section pop up and "MU2" label text from profile dialog removed.

#### SITE V2.4 | Released on: 11/30/2016
* Updated Reference C-CDA Validator to fix content validation for Labs/Vitals/Procedures/Immunizations.
* Upated FHIR Sandbox to fix error handling and displaying appropriate error messages and editing of clients.
* Updated Scorecard to incorporate feedback from Internal ONC team on decoupling the various validations and its results.
* The new SITE UI Makeover Release has been updated to have the ONC Tech Lab Themes and Layouts.

##### ETT V1.1.3.1 | Released on: 11/28/2016
* XDR SAML validation is available at ETT - migrated from TTT.
* HISP XDR Sender Test 12: XDM metadata now conformant
* XDS toolkit updated to version 4.

#### ETT V1.1.3 | Released on: 11/17/2016
* Final-Recipient field for MDNs returned by ETT now conform per RFC 3798 Section 3.2.4 to use message recipient (earlier it was pointing to the sender).
* The failure message tracking cases now pass only if X-Original-Message-ID can be correlated and do not fallback to In-Reply-To anymore
* XDM limited metadata fixed for the issue reported and is referenced from github now.
* UI Enhancements
    * After clicking More Info/Log links from the test case, the back button navigates back to the corresponding test case.
    * Labels changed to "XDM Validator" & "XDR Validator".
* FAQ page added [https://ttpedge.sitenv.org/ttp/#/edge/faq] (can also be accessed directly from here: https://github.com/onc-healthit/ett/wiki/FAQ)
* CCDA validator updated to 1.0.7 [https://github.com/onc-healthit/referenceccdavalidator/releases]

#### SITE V2.3.9 | Released on: 10/31/2016
* Updated C-CDA Validator to version 1.0.5
* Updated FHIR Sandbox with bug fixes based on feedback and comments on Alpha Release.
* Updated DS4P Test Data PDF and Test XML files.
* Provided the new SITE UI Re-design concept.

#### ETT V1.1.2 | Released on: 10/20/2016
* HISP XDR Sender Tests 11 and 12: XDM metadata sent by ETT is now conformant
* File selection dialog display fixed to show html as files instead of folders.
* 'More Info.' section missing description for XDR test cases now added.
* The "Step 1" instruction in the XDR test case has been fixed to have increased clarity.
* Server configured to run the MDHT validator on a separate instance for better performance.

#### ETT V1.1.1 | Released on: 10/06/2016
* ETT User guide updated and is available from the github repository.
* ETT Public Root CA download from the Direct component fixed to point to sitenv.org.der.
* SMTP HISP MT tests use X-Original-Message-ID  (earlier used In-Reply-To, now only as a fallback) header for failure DSNs
* SMTP test case descriptions are configurable from a JSON file in the application directory.
* XDR MT 38: referenced endpoint updated from processedonly to processeddispatched for correct behavior and the logs show the asynchronous notification.
* References to previous ETT Instruction/Demonstration Videos have been dropped
* HISP MT SMTP/SMTP cases description changed to reflect the limitation
* Direct Page ETT Certificate tool tips updated to relevant names
* Validation report for profile now lists the test result in a sorted order by date
* DCDT is accessible from the menu inside Direct component.
* The direct validation report link URL port reference removed.

#### ETT V1.1.0.1 | Released on: 09/30/2016
* UI change: XDR TLS certificates from the UI now point to the github location:    
  * https://github.com/onc-healthit/ett/blob/resources/certificates/common/xdr-tls/keyAndCert.zip
* Direct send decryption issue reported has been fixed which involves
  * Java Cryptography Extension (JCE) key strength update in the environment
  * The encryption library points to the right version
* Environment updated so that the TTP mail server allows MAIL FROM differing from AUTH information.

#### SITE V2.3.8 | Released on: 09/26/2016
* Updated SITE Scorecard URL.
* Deployed Alpha Release of SITE FHIR Sandbox.
* Deployed Alpha Release of SITE DS4P Validator.
* Deployed Updates to C-CDA Validator which includes test data, test xml files, vocabularies and HL7 errata.

#### ETT V1.1.0 | Released on: 09/22/2016
*For SUT Receiver Test Cases: XDR Test 3, SMTP MT-39, SMTP MT-40 and SMTP MT-41, the C-CDA Document Selection dialog now automatically sets the context to select documents required for testing.
 * https://ttpedge.sitenv.org/ttp/#/edge/xdr (XDR Test 3)
 * https://ttpedge.sitenv.org/ttp/#/hisp/mu2 (SMTP MT-39, SMTP MT-40 and SMTP MT-41)
* Changed the TTP Footer notice about browsers from "Recommended Browsers: For best result use, Firefox 3.x and Chrome" to “Tested with Firefox 3.x and Chrome browsers.”
* Resolved TEXT WRAP Issues for C-CDA vocabulary results where the results were not wrapping earlier and will get wrapped properly.
* Added descriptions to XDR Test Cases 19, 48, 49, 20a/20b, 50a/50b which is available when “More Info” is clicked.
* Message Validator UI changes:
  * Removed the Sender / Receiver selection for Step 3 of the validation.
  * Added checks to ensure context is set (Validation Objective and Reference File Name) before allowing documents to be validated.
* C-CDA Document Selection Dialog
  * Removed the Sender/Receiver selection button since the test cases provide the necessary context of Sender or Receiver. As a result, the files that need to be used are shown based on a Sender or Receiver Test Case.
* For HISP Sender SMTP Tests 1-8, 14 (Send), added clarification to the narrative to indicate that the C-CDA document type selected for validation does not affect the test result.
* For Edge Sender SMTP Tests 1-8, 14, 18 (Send), added clarification to the narrative to indicate that the C-CDA document type selected for validation does not affect the test result.
* Also corrected the test cases in the description for Edge Sender SMTP Tests 1-8, 14,18 (Send) to include all the test case numbers.

#### SITE V2.3.7 | Released on: 09/09/2016
* Added 'Try Me' Feature.
* Improved Error Handling and User Notification.
* Updated UI.
* Fix for Effective Time validation when present in seconds format. 

#### ETT V1.0.23 | Released on: 09/08/2016
* SMTP
  * Receiving HISP MT case exception due to corrupt email in the RI inbox fixed; this also enhances the MT cases to be able to run simultaneously
  * Announcements to the footer added
  * Other fixes include new footers, release notes link in the footer, show all registered direct addresses list, 
	* validation result order, errors from more info, xdr validator dropdown
* Displaying the correct validation status (passed/failed) for SMTP and XDR cases
  * Baselines all the changes from the NIST 1.0.22 release

#### SITE V2.3.6.2 | Released on: 08/19/2016   
* Addition of Unique Instance Identifier rule in SCORECARD under Miscellaneous Section.
* IG References for issues change dynamically based on type of document processed(R1.1, R2.1).

#### ETT V1.0.22 | Released on: 8/15/2016
* Direct
  * Added SHA-256 signature algorithm selection on Direct send page.
  * Fixed the different trust anchor certificate on Direct send.
* XDR
  * Removed XDR 4c and 15c.
  * HISP, Your System As Receiver: Updates to allow the outgoing "Direct From" address to be configurable from the UI.  This affects: XDR 13, XDR 14, XDR MT Test 15, XDR MT Test 16, XDR MT Test 30, XDR MT Test 31, XDR MT Test 32, XDR MT Test 33, XDR MT Test 34, XDR MT Test 35, XDR MT Test 36, XDR MT Test 37, XDR MT Test 38, XDR MT Test 43, XDR MT Test 44.
  * Removed XDR 4c and XDR 15c.  Full explanation is available here: https://groups.google.com/forum/#!topic/edge-test-tool/v7DTivWWdR8
* C-CDA R2.1 Validator
  * Corrected a display issue where a green check was in some situations showing when the XML contained errors.
* IMAP
  * HISP, Your System As Sender: IMAP 9 updated to allow a greater flexibility of error messages from SUT

#### SITE V2.3.6.1 | Released on: 08/09/2016
* Fixed time validation routine to not reduce scores when additional precision is specified as part of the time element.

#### SITE V2.3.6 | Released on: 08/05/2016
* File contents are no longer encoded.
* File contents are sent as an attachment in using optimized XOP message.
* Full and minimial messages are sent correctly when selected from dropdown.

#### SITE V2.3.5 | Released on: 08/05/2016
* Added ability to save the scorecard results to PDF.
* Added context to IG References to Standards.
* Added HL7 Example Task Force links to Best Practice links.
* Scoring for documents is optimized in case of any section is null flavor.
* Updated vital sign UCUM validation to validate against its value set.
 
#### SITE V2.3.4 | Released on: 08/04/2016
* C-CDA Validator Update
* Latest MDHT build.
* LOINC displayname validation is now done against the LONG_COMMON_NAME rather than COMPONENT.
* Vocabulary bug fixes.
* C-CDA IG validation bug fixes.
* Reference Content validation bug fixes.
 
#### ETT V1.0.21 | Released on: 07/27/2016
* SMTP
  * Fix whitespace issue in MDNs for 39, 40 , 41
* C-CDA R2.1 Validator
  * Fix display issue: green check when there are errors with C-CDA validator

#### ETT V1.0.20 | Released on: 07/20/2016
* MU2
  * Added attachments for MU2 39, 40 and 41

#### SITE V2.3.3 | Released on: 07/15/2016
* Added full support for C-CDA R1 to Scorecard - The Scorecard now fully supports scoring of documents that conform to either the  C-CDA R1.1 or the C-CDA R2.1 Implementation Guide.

#### SITE V2.3.2.1 | Released on: 07/08/2016
* Applied Scorecard hotfix - Fixed null flavor with problem status code throwing service error

#### SITE V2.3.2 | Released on: 06/28/2016
* Updated Reference C-CDA Validator - Updated Reference Validator to display content errors based on certification test data scenarios

#### SITE 2.3.1 | Released on: 06/28/2016
* ONC C-CDA Scorecard (Beta) release
* Added Calculation of Industry Average (based on average of all scores since scorecard was made available)
* Updated method of counting issues discovered
* Enhancements for scoring both C-CDA R2.1 and R1.1 documents 
* Enhancements to section heatmap 

#### ETT V1.0.19 | Released on: 6/24/2016
* XDR
  * XDR 7: Additional testing of socket to verify no information is being sent across after bad certificate is provided.
* C-CDA R2.1 Validator
  * Added warning pop-up when C-CDA reference filename was not selected before validation process.

#### ETT V1.0.18 | Released on: 6/21/2016
* XDR
  * The tool will now look for the metadata-level element as either a top-level element in the SOAP headers or within the Direct Address Block.
  * Additional checking and logging of the socket in XDR Test Case 7. Also adds a delay.
  * Minor metadata cleanup.

#### ETT V1.0.17 | Released on: 6/13/2016
* XDR
  * Fixed display bug for XDR endpoints.
  * XDR 1 -- The metadata is now validated by the tool automatically rather than needing to be uploaded to TTT manually.  The C-CDA validaton report is also available without needing to be uploaded manually.
  * XDR 2 -- The metadata is now validated by the tool automatically rather than needing to be uploaded to TTT manually.
  * XDR 3/5 -- RegistryResponse is now automatically checked, no longer manually check needed for "success".
  * XDR MT 49 -- Direct Address Block now automatically validated.
* XDM
  * Added standalone validator for XDM.
* Direct
  * Added validation for XDM payload.
* C-CDA Validator
  * Fixed display issue for success validation.
* Database
  * Updated table XDRRecord to add C-CDA report field. If you are updating from a previous version, run this: "ALTER TABLE XDRRecord ADD MDHTValidationReport LONGBLOB;"

#### SITE 2.3.0.1 | Released on: 06/08/2016
* Scorecard Hot fix for CDN/Broken link Issue

#### ETT V1.0.16 | Released on: 5/18/2016
* SMTP
  * Updated description for SMTP Test 13

#### SITE V2.3.0 | Released on: 5/16/16
* C-CDA Validator Service Release
  * Fixed concurrency issue
  * Updated valuesets and validator configuration
* C-CDA Validator Portlet
  * 508 compliancy work
* Direct Transport Portlet
  * Addressed issues where x.509 certificates were being improperly loaded
* C-CDA Scorecard initial release

#### ETT V1.0.15 | Released on: 5/13/2016
* SMTP
  * Added new MT case 41
* XDR
  * Bug Fix for XDR MT 38.

#### ETT V1.0.14 | Released on: 5/4/2016
* XDR
  * Bug Fix for XDR MT 19/48, was not consistently tracking MessageID.
* SMTP
  * Language cleanup on test case descriptions.
* Misc
  * Minor bug fixes and improvements.

#### ETT V1.0.12 | Released on: 4/21/2016
* XDR
  * XDR 4 - sends XML attachment now.
  * XDR 4 - better error reporting.

#### ETT V1.0.11 | Released on: 4/20/2016
* XDR
  * Corrected XDM file-name length issue in XDR
  * Corrected mismatch in outgoing XDR messages (ID of metadata did not match ID of document)

#### ETT V1.0.10 | Released on: 4/15/2016
* SMTP
  * Added MT SMTP cases 18(a) and 47(a)
  * Checking Disposition-Notification-Oprions header for dispatchedonly-plain endpoint
  * Text change for noaddressfailure9-plain endpoint
* XDR
  * For sending of XDR Direct Disposition, Direct Address Block now contains relatesTo field
  * Parser now strips the 'mailto:' from the direct address in the XDR direct address block

#### ETT V1.0.9 | Released on: 4/12/2016
* SMTP
  * For SMTP Test Cases MT18/MT47, now enables the use of STARTTLS for sending of MDNs

#### ETT V1.0.8 | Released on: 4/11/2016
* XDR
  * Fixed XDR message, direct block was not properly added

#### SITE V2.2.7 | Released on: 4/8/16
* C-CDA Validator Service Release
  * Problem Observation Valuesets
  * Vocabulary validation severity can be configured to be SHALL, SHOULD, MAY severity
  * CDT Codesystem is loaded but not yet configured
  * New MDHT Build

#### ETT V1.0.7 | Released on: 4/8/2016
* XDR
  * Removed XDR 4d, 4e and 15d, 15e
  * XDR 13 now sends sample C-CDA payload for use in packaging XDM
  * Removed all routing information from metadata for test case XDR 4c and 15c
  * Corrected a typo in the routing addresses used in XDR 15d
  * Added asynchronous possibility for test case MT 13-16, 32-37, 42 and 43
* SMTP
  * Bug fix for MT 3
  * Updated endpoints for MT 18 and MT 47

#### ETT V1.0.6 | Released on: 3/22/2016
* Message Tracking
  * MT 18/47 Endpoints Updated Removal of MT 22, 41 and 42 Removal of IMAP/POP 22
* Direct 
  * Fixed smtp MDN when no MX record has been discovered. It now send to the hostname

#### ETT V1.0.5 | Released on: 3/21/2016
* SMTP
  * Check both failure MDNs and DSNs
* Message Tracking
  * MT 39 - Check both processed and dispatched MDNs
  * MT 40 - Check for processed MDNs with no x-header in dispatched MDN
  * MT 45 - Check for both unique Ids and disposition notifications header
* Direct
  * Fixed problem when trying to pull encryption certificate by DNS/LDAP. If an exception was thrown during the lookup the Direct message was not sent.

#### ETT V1.0.4 | Released on: 3/02/2016
* SMTP
  * MIME Type updates on SMTP cases 25b, 25d, 25e and 29
* XDR
  * Fixed a double base64 encoding bug that was occurring in some test cases
* C-CDA Widget
  * Fixed Cancel button for C-CCDA Widget
* Direct
  * Certificate links on Direct main page are now configurable via a file

#### SITE V2.2.6 | Released on: 2/29/16
* C-CDA Validator Service Release
  * Improved validation performance, most validations should take under 1 minute.
* XDR Validator Service Release
  * Responses are now in MTOM format
  * Fixed where some nodes were not found due to incorrect Qnames.

#### ETT V1.0.3 | Released on: 2/25/2016
* SMTP
  * POP-1,2 perform AUTH before NOOP
  * POP 12 fixed to handle empty UIDL issue with Apache James

#### ETT V1.0.2 | Released on: 2/19/2016
* Direct
  * Links for Direct certificates on Direct Home page are now configurable for ETT local installation
* SMTP
  * Message Tracking logs shows time taken to get back an MDN
  * Bug fix for Message Tracking timeout cases

#### ETT V1.0.1 | Released on: 2/11/2016
* SMTP
  * Description updates for SMTP/IMAP/POP test cases
  * From address change for all SMTP receive cases i.e the from address will be the same as to address. (Earlier the from address was wellformed1@hit-testing2.nist.gov). The descriptions for this cases have been changed accordingly

#### SITE V2.2.5 | Released on: 1/31/16
* New MDHT Release for IG conformance
* Vocabulary Updates to include Non-VSAC value sets
* Reference CCDA IG updates
* Test Data updates for C-CDA certification criteria

#### ETT V1.0.0 | Released on: 1/21/2016
* SMTP
  * UI change for receiver test
  * Bugfixes for Message Tracking cases
  * Added SMTP Message tracking cases

#### ETT V0.0.10 | Released on: 1/13/2016
* MDN
  * Added empoints for bad MDNs generation
* C-CDA
  * Added link to C-CDA R2.1 test samples repository
  * Added Direct message endpoints for C-CCDA R2.1 validation

#### SITE V2.2.4 | Released on: 12/23/2015
* C-CDA Validator Release
* MDHT Update
* UI Update
* Added Test Data Repository

#### ETT V0.0.9 | Released on: 12/15/2015
* Message validator
  * Added widget to select CCDA R2.1 samples and objectives
* Edge
  * Added Message Tracking, POP and IMAP test cases
  * Added MIME type tests, tests with multiple attachments and content validation

#### SITE V2.2.3 | Released on: 12/09/2015
* Upgraded C-CDA 2.1 Validator
* Deployed new C-CDA valuesets and updated configuration(s)
* Extended validator and Reference validator with separate R1 and R2 configurations
* Updated validators and valueset/codes to enable configuration for path expression
* Added DVT FAQs
* Added 2015 DCDT
* Updated Direct Sandbox Links

#### SITE V2.2.2 | Released on: 10/30/2015
* Upgraded SITE C-CDA Validator
  * Added the Reference C-CDA Validator functionality for R2.0
  * Added vocabulary valueset validation for new code system files
  * Added vocabulary valueset validation for new value sets available from VSAC

#### ETT V0.0.8 | Released on: 10/06/2015
*ETT
 * Added CCDA R2 Validator
* Direct
 * Added CCDA R2 validation to Direct validator
 * Improved error display on Direct Validation report

#### SITE V2.2.1 | Released on: 09/27/2015
* Upgraded SITE C-CDA Validator from R2.0 to R2.1
* Retired SITE QRDA Validator

#### SITE V2.2.0 | Released on: 08/17/2015
* Added finalized 508 Compliance UX
* Added Vocabulary Validation to the C-CDA Validator
* New version of SITE Direct Transport Standard Testing Services (1.1)
* New C-CDA R1.1 and R2.0 builds
       
#### SITE V2.1.0 | Released on: 07/10/2015
* Added the SITE Direct Transport Standard Testing Services

#### ETT V0.0.7 | Released on: 06/12/2015
* Direct
  * Improved error reporting for DTS 195 when Body contains non ASCII characters.
* XDR
  * Added test case 4e

#### ETT V0.0.6 | Released on: 05/27/2015
* XDR
  * Added XDR MU2 tests.
  * Updated descriptions for the XDR test cases.

#### ETT V0.0.5 | Released on: 05/11/2015
* SMTP
  * Added download link for SMTP attachments in the log.

#### ETT V0.0.4 | Released on: 05/05/2015
* SMTP
  *	Updated test cases 46.
  *	Fixed the exception error for test case 13.
  * Better logs for negative test cases (10,11,13,17).

#### SITE V2.0.4 | Released on: 05/01/2015
* Updated Virtual Machines to fix the GHOST flaw
* Increase VM disk size

#### SITE V2.0.3 | Released on: 04/30/2015
* Added the CYPRESS QRDA Validator to the Quality Reporting Standard Sandbox and Testing Resources Pages

#### SITE V2.0.2 | Released on: 04/17/2015
* Added the SITE Direct SMTP Edge Test Tool
* Added optional parameters to the SITE Direct XDR Edge Test Tool
* Fixed issues in formatting of a Provider Directory response
* Completed additional required Section 508 Accessibility Issues
* Added Bonnie to the CQM Sandbox
* Added Public Health Reporting, Laboratory Standards, Electronic Prescribing, and SOAP Transport Sandboxes

#### ETT V0.0.3 | Released on: 03/10/2015
* Direct
  * Added DNS lookup for address bound encryption certificates.
  * Added LDAP lookup for address and domain bound encryption certificates.
* XDR
  * Added Cancel button to XDR tests.
* SMTP
  * Fixed few minor bugs.
  * Added Cancel button to XDR tests.

#### ETT V0.0.2 | Released on: 03/03/2015
* Direct
  * Changed subject validation from Warning to Info when message is wrapped
  * Added validation Content-transfer-encoding (DTS 136-148-157) and Body (DTS 195) which were missing
  * Fixed bug where XDM zip attachment could not be downloaded
  * Fixed bug with quoted-printable encoding, part was recognized as plain text
* Direct listener
  * Fixed bug when sending two messages through the same connection. The listener now returns an error 421 and close the connection if the system tries to send more than one message.
* XDR
  * ETT is now using fixed endpoints when ETT is receiving XDR and users need to provide Direct from address to corelate the XDR message.
* Misc. ETT
    * Added favicon

#### SITE V2.0.1 | Released on: 02/26/2015
* Added the SITE Direct XDR Edge Test Tool

#### SITE V2.0 | Released on: 12/31/2014
* Refactored all of the SITE portlet code
* Updated SITE C-CDA Validator to version 2.0
* Updated SITE Direct Transport Test Tool to version 2.0
* Updated SITE Provider Directory Test Tool to version 2.0
* Updated SITE QRDA Validator to version 2.0

#### SITE V1.3.9 | Released on: 12/26/2014
* Updated SITE Provider Directory Test Tool to version 1.1

#### SITE V1.3.8 | Released on: 11/11/2014
* Incorporated the CQM Certification Sandbox
* Updated look and feel of the SITE application

#### SITE V1.3.7 | Released on: 10/01/2014
* Incorporated the Direct Certificate Discovery Tool

#### SITE V1.3.6 | Released on: 07/30/2014
* Updated the look and feel of SITE to support Section 508 Compliance

#### SITE V1.3.5 | Released on: 07/18/2014
* Updated the C-CDA validation service (new MDHT build)

#### SITE V1.3.4 | Released on: 07/10/2014
* Incorporated SITE Statistics for existing portlets

#### ETT V0.0.1 | Released on: 07/09/2014
*ETT
 *Initial add of the release notes
*Direct
 *Initial add of DIRECT from TTT code
*SMTP
 *Initial add of SMTP module
*XDR
 *Initial add of XDR module	

#### SITE V1.3.3 | Released on: 06/13/2014
* Updated C-CDA Validator to version 1.5

#### SITE V1.3.2 | Released on: 05/01/2014
* Updated SITE to address the potential Heartbleed issue.

#### SITE V1.3.1 | Released on: 04/08/2014
* Addressed defects in both the Provider Directory Test Tool and the QRDA Validator

#### SITE V1.3 | Released on: 03/06/2014
* SITE Usability Updates

#### SITE V1.2 | Released on: 01/28/2014
* Addition of Federated HPD and QRDA sandboxes

#### SITE V1.1 | Released on: 06/30/2013
* Addition of the Direct Sandbox

#### SITE V1.0 | Released on: 04/09/2013
* Addition of the C-CDA Sandbox

# The Standards Testing & Implementation Environment (SITE)
## Release Notes

#### V 3.1.66 | Released on: 03/27/2023
* C-CDA Validator
  * fill in here Girish 
  * fill in here Prabhu
  * fill in here Dragon
* ETT
  * Remove DCDT fill in here Girish
* General
  * Infrastructure updates

#### V 3.1.65 | Released on: 02/27/2023
* C-CDA Validator
  * Update SubstanceReactantForIntolerance value set to include the latest codes from VSAC 	
* Direct
  * Fix drop downs not loading for "Select a Discovery Test Case"
  * For Direct: 4.0, add ability to send a direct message using a certificate that does not have a CRL
* General
  * Infrastructure updates
  
#### V 3.1.64 | Released on: 01/09/2023
* Direct
  * Add Direct version 1.3 to ETT
  * Add SVAP 2022 DCDT to ETT
* Other
  * Fix broken links in SITE test-tools page

#### V 3.1.63 | Released on: 12/05/2022
* C-CDA Validator
  * Add table explanation to the ETT validator home which relates certification criteria version with C-CDA and USCDI version: https://ett.healthit.gov/ett/#/validators
* FHIR
  * R4 dependency update for bulk R4
* Other
  * Various Direct and other server infrastructure upgrades and fixes
  * Fix ETT GG issue, "XDR Endpoint with TLS not working"

#### V 3.1.62 | Released on: 09/29/2022
* C-CDA Validator
  * Correct template versions for Problem Status and Allergy Status to 2019-06-20
  * Relax severity of value set constraint on Provenance Author Participation to match IG
  * Update scenarios for SVAP-2022 to match test data for inpatient samples
* FHIR
  * Update navigation links in R4 Bulk data pages
  
#### V 3.1.61 | Released on: 08/31/2022
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

#### V 3.1.60 | Released on: 07/25/2022
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

#### V 3.1.59 | Released on: 05/31/2022
* C-CDA Validator
  * Improve validator backend service uptime
  * Further improve Artifactory uptime (C-CDA dependency server)
* FHIR
  * Fix incompatible character encodings UTF-8 and ASCII-8BIT for US Core Encounter Profile 
  * Update dependencies Spring, Spring-security-web, and JUnit
  * Remove FHIR Query Tool and FHIR Conformance Test Tool

#### V 3.1.58 | Released on: 04/25/2022
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

#### V 3.1.57 | Released on: 03/28/2022
* C-CDA Validator
  * Update value set 2.16.840.1.113883.3.88.12.80.62 Vital Sign Result Type to the latest version in order to allow the use of code 3150-0
  * Update test data to change Allergy Drug Class to a value in the Value set for b1, e1, g9 criteria. The sender pdf files have been updated
  * Update CIRI (b2) test data instructions to allow the reconciliation of an Allergy due to a drug class
* FHIR
  * Update R4 CapabilityStatement with absolute URLs if they are not fragment references (/fhir/metadata) 

#### V 3.1.56 | Released on: 02/28/2022
* C-CDA Validator
  * Add regulation clarification to configuration
  * Fix ActStatus Value Set OID in configuration from 2.16.840.1.113883.1.11.159331 to 2.16.840.1.113883.1.11.15933
* General
  * Update server infrastructure
* FHIR
  * Remove reference to STU3 and reference to DSTU2 from fhirsandbox

#### V 3.1.55 | Released on: 01/31/2022
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

#### V 3.1.54 | Released on: 12/27/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Update linked reference mismatched org name message for clarity and specificity
  * Fix recent server configuration issue which may have suppressed certain vocabulary results
  * Add missing CDA Extensions from 2018: sdtc:asPatientRelationship, sdtc:deceasedInd, sdtc:deceasedTime, sdtc:multipleBirthInd, sdtc:multipleBirthOrderNumber, sdtc:statusCode and stdc:desc
  	* See https://confluence.hl7.org/display/SD/CDA+Extensions for a detailed description of the extensions
  * Limit Vital Sign Observation/value to data type PQ
  * Update value set for Marital Status to include U: Unmarried and C: Common Law
  * Report only one validation issue (versus two issues) for an incorrect or missing Allergy Section Code

#### V 3.1.53 | Released on: 12/06/2021

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
 
#### V 3.1.52 | Released on: 10/25/2021

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

#### V 3.1.51 | Released on: 09/27/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Relax participant constraints to allow free-text names in Referral Note as part of new MDHT 20210924 Release
  * Update 170.315(e)(1) Inpatient setting Sample 1 files to include Reason for Referral instructions to enable vendors to create Referral Notes
* SITE-UI
  * Fix 'Original C-CDA' tab display issue in CURES SITE C-CDA Validator
* ETT
  * Update ETT dependencies as per dependabot
  * Fix potential SQL injection issues in ETT

#### V 3.1.50 | Released on: 08/30/2021

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
   
#### V 3.1.49 | Released on: 07/26/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Add linked reference support for Note Activity
  * Implement Errata 2041: Allow for Advance Directive organizer or Advance Directive observation in an Advance Directive section but prevent an entry from having both an     observation and an organizer
  * Update ValueSet HL7 RefrainPolicy 2.16.840.1.113883.1.11.20446 to reflect the DS4P IG
  * Updated dependencies for security
* SITE-UI
  * Fix xdr message sender endpoint
 
#### V 3.1.48.1 | Released on: 07/02/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Add support for linked references in author when validating provenance representedOrganization/name (with the exception of Note Activity)
  * Remove XML files from e1 criteria for inpatient

#### V 3.1.48 | Released on: 06/28/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Remove XML Line number and XPath from Content Validation results 
  * Add logic to allow Notes Activities to be present in any section within the C-CDA document 
  * Relax Care Team section requirement to warnings instead of errors
  * Update Gold Samples for Sample1 and Sample2
  * Fix bug in the CPT Loader where some records were missing

#### V 3.1.47 | Released on: 06/02/2021

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Updated Content Validator to allow notes activities in specific sections which include Lab Results, Procedures, Notes and Encounters
  * Updated Error Messages for Notes Provenance Entries
  * Updated Provenance Validation for Inpatient setting for Jane Clarkson to have the right organization name
  * Updated Sample1 and Sample2 files to include Clinical Notes validation

#### V 3.1.46 | Released on: 04/26/2021

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

#### V 3.1.45 | Released on: 04/05/2021

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

#### V 3.1.44.1 | Released on: 03/08/2021

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

#### V 3.1.44 | Released on: 02/22/2021

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

#### V 3.1.43 | Released on: 01/25/2021

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
  
#### V 3.1.42 | Released on: 12/07/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Add IG-level UDI validation
  * Add Provenance content validation for section and entry relationships
  * Update CDT, CPT, LOINC, SNOMED, and RXNORM code systems
  * Fix Care Team cardinality and severity issues (4435-152, 4435-166, etc.)
  * Fix Note Types translation code issue where our value set was out of date (3250-16940, 3250-16941)
  * Fix cardinality and remove 'such that it' for Note Activity Author Participation (3250-16913)

#### V 3.1.41.1 | Released on: 11/16/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Updated value sets to the latest available from VSAC (for the CURES option)
  * Fixed telecom validation to validate numbers only
  * Fixed issue where the Reference Validator was not producing a log
  * Removed excess cache info and warnings from log
  * Updated JDK version notes in Reference Validator readme

#### V 3.1.41 | Released on: 10/27/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
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
  
#### V 3.1.40 | Released on: 09/28/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Updated USCDI Sample 3 Test Data for Ambulatory and Inpatient to correct date of birth and timing errors.
  * Updated Notes Error reporting and fixed errors related to Sample 3 for Ambulatory and Inpatient settings.
  * Updated Author Provenance Error Reporting.
  * Changed Telecom and Birth Sex Error reporting from WARNING to ERROR.
* Scorecard
  * Resolve issues when parsing a document with multiple patient names where one does not have a legal use.
  * Update support email to edge-test-tool@googlegroups.com.

#### V 3.1.37.1 | Released on: 09/15/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * Renamed the test data files to start from version 1.
	 * Updated the test data to include USCDI elements as part of Sample3 files.
	 * Updated Sample3 for b1, e1 and g9.
	 * Updated DS4P test data to include entry level markings. 

#### V 3.1.37 | Released on: 06/29/2020

#### C-CDA Sandbox Updates:
* C-CDA Validator
  * DS4P update to the 'CURES' Reference C-CDA Validator 
    * Reviewed and updated DS4P validations based on HL7 Reaffirmation Status
  * Content-related cures updates to the 'CURES' Reference C-CDA Validator
    * Updated C-CDA Validator with changes to detect conformance to Notes sections and Notes entries for compliance to US CDI

#### V 3.1.36 | Released on: 06/01/2020

#### C-CDA Sandbox Updates:
* __Scorecard 2.0__ (Released on: 06/03/2020)
  * Support the latest rubrics/new Scorecard rules developed over the past year
  * Support CURES validation within the Scorecard
  * Update UI
* C-CDA Validator
  * Add 2015 Edition Cures Update R2.1 Validator support to the C-CDA Validator
  
#### V 3.1.35 | Released on: 04/27/2020

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

#### V 3.1.34 | Released on: 03/30/2020

#### C-CDA Sandbox Updates:
* None.

#### V 3.1.32 | Released on: 01/27/2020

#### C-CDA Sandbox Updates:
* None.

#### V 3.1.31| Released on: 11/22/2019

#### C-CDA Sandbox Updates:
* UI C-CDA Validator update to provide proper error when server is down.

#### V 3.1.30| Released on: 09/30/2019

#### C-CDA Sandbox Updates:
* Fixed github vulnerabilities.
* Udated github link to new repository.
* Add support for vocabularyValidationConfigurationsErrorCount.
* Adds tracking for errors only in total vocabulary validations run.

#### FHIR Sandbox Updates:
* Added page title to client login and client registration pages.    


#### V 3.1.29 | Released on: 08/26/2019

#### C-CDA Sandbox Updates:
* None.

#### V 3.1.28 | Released on: 07/29/2019

#### C-CDA Sandbox Updates:
* Add severityLevel support to the C-CDA Validator UI
  * Adds the ability to select a severity level limitation for results returned. The user can now select the desired severity or severities. Selecting "Errors, Warnings, and Info" processes all available result types and is the default setting. The remaining selections limit the results as stated and should subsequently offer faster results".
* Support severityLevel limiting on the content validator in addition to prior support for the code validator and reference validator via the 'severityLevel' flag in a POST call.

#### FHIR Sandbox Updates:
* Added Provenance resource 
* Updated R4 to support additional search capabilities for Careplan, Condition, Devices, Encounter, Goal, Immunization, Medication Statement, Pediatric Weight For Height, Observation Lab, Smoking Status and BMI For Age resources. 
 * Bug fixes for DSTU2 and R4



#### V 3.1.27 | Released on: 06/24/2019

#### FHIR Sandbox Updates:
* Added delete client capabilities.
* Updated OpenID connect with introspection endpoint.

#### C-CDA Sandbox Updates:
* The C-CDA Validator now indirectly supports UTF files encoded with a BOM by removing the BOM before processing.
* The Reference C-CDA Validator API and static UI in local instantiations now support limiting MDHT Conformance and Vocabulary Validation results via their severity (Content limiting is coming soon). This has the potential to offer significant performance gains for users only interested in specific types of results, expecially on larger or issue-prone files. To use the feature, either use the static UI, or, send body form-data key:severityLevel and value:ERROR, WARNING, or INFO. Please note that selecting INFO will return all results, WARNING will return warnings and errors, and ERROR will return errors only.

#### V 3.1.26 | Released on: 05/27/2019

#### FHIR Sandbox Updates:
* Updated EHR Launch Sequence Software to resolve defects when testing with Inferno by redirecting the launch correctly.
* Updated OpenID capabilities to pass Inferno testing.
* Fixed EHR Launch Sequence to pass Inferno testing.
* Updated Refresh Token sequence to return patient Ids.
* Updated Github with R4 Release.
* Updated FHIR Sandbox with test data to pass Inferno tests.

#### C-CDA Sandbox Updates:
* None.

#### V 3.1.25 | Released on: 04/29/2019

#### FHIR Sandbox Updates:
* Updated FHIR DSTU2 Server to allow Inferno to test SITE FHIR Server for Program Edition.
* Supported the Standalone Patient Launch Sequence.
* Added capabilities for EHR Launch Sequence.
* Fixed Password Reset capabilities.
* Added OpenID capabilities to the FHIR Server.

#### C-CDA Sandbox Updates:
* Updated C-CDA Configuration to fix Reference Validator Reboot issues on AHRQ Server.

#### V 3.1.24 | Released on: 03/25/2019

#### C-CDA Validator Updates:
* A unit can now be equal to '1' in certain scenarios when it is selected from the UCUM value set. For local instantiations, the configuration is up to the user to apply with the new UnitAllowsOneValidator.
* CONF:1198-8559 was updated to enforce the if portion of the rule, "If Observation/value is a physical quantity (xsi:type="PQ"), the unit of measure SHALL be selected from ValueSet UnitsOfMeasureCaseSensitive (2.16.840.1.113883.1.11.12839) DYNAMIC
(CONF:1198-8555)."
* Updated doseQuantity/@Unit from the invalid value 'mg/actuat' to the valid UCUM value 'mg'.
* Updated value datatype in Result Observation (V3) from PQ to ST for 170.315_b1_toc_amb_ccd_r21_sample1_v12.xml and 170.315_b1_toc_amb_rn_r21_sample1_v12.xml. Note: due to this change, these file are now v13.
* The Reference C-CDA Validator and Code Validator API documentation material was updated to enhance the clarity for setting up local installations.

#### V 3.1.20 | Released on: 10/29/2018

#### C-CDA Validator Updates:
* Updated C-CDA Vocabulary Validator to match proper configuration paths and dynamic value sets where it was erroneous.
* Updated Test Data to remove external document reference from CarePlan.
* Updated Test Data to add R1.1 Template Id for Encounter Diagnosis to the DS4P Samples.

#### FHIR Sandbox:
* Updated DSTU2 Server to pass Inferno for Conformance Resources and for other specific clinical resources.

#### V 3.1.19 | Released on: 9/24/2018

#### FHIR Sandbox Updates:
* Updated FHIR sandbox with fixes to Bulk Data APIs.
* Added Inferno Testing Tool to SITE UI.

#### V 3.1.18 |   Released on: 8/27/2018

#### C-CDA Validator Updates:
* Updated C-CDA Value Sets from VSAC to use the 6-15-2018 version instead of the older versions.
* Fixed Test Data to ensure no errors in samples based on the value set update.

#### V 3.1.17 |   Released on: 7/30/2018

#### C-CDA Validator Updates:
* Substance Reactant Value set was updated to the latest value set from VSAC.
* Added support for the latest LOINC.csv file to enable both 2015 baseline and newer versions of LOINC codesystem files.
* Updated VDT Test data XML file to remove errors from ERRATA update.

##### FHIR Sandbox Updates: 
* Updated FHIR Sandbox with Bulk API capability sample code and tutorials.

#### General SITE Updates:
* Updated SITE Contact Email to SITTeam@hhs.gov 

#### V 3.1.16 |   Released on: 6/25/2018

#### C-CDA Validator Updates:
* An invalid error no longer fires for recordTarget/PatientRole/Patient/Guardian when no code exists. The terminology portion of the error CONF:1198-5326 should only fire if the code exists and the terminology is invalid but was previously firing without a code.
* Added support for loading custom vocabulary configs in realtime.

#### V 3.1.15 |   Released on: 5/29/2018

#### C-CDA Validator Updates:
* The validator has been updated to include the latest HL7 C-CDA Schema (with internal fix due to errata in HL7 Schema) which includes support for sdtc:functionCode in cda::Performer2 and cda::Participant2

#### C-CDA Scorecard / One-Click Scorecard Updates: 
* The scorecard has been updated to deduct points if the entire time element is padded to zero. For example: "19700501000000+0000" or "19700501000000-0000"

#### V 3.1.14 |   Released on: 4/30/2018

#### C-CDA Validator Updates:
* C-CDA Validator was updated to include HL7 approved September 2017 ERRATA for C-CDA R2.1. For more information please refer to https://groups.google.com/forum/#!topic/edge-test-tool/vsA_W9Yg4mc
* Test data was updated to make them conformant to the new ERRATA.
* Validator was updated to include document type validation for certification criteria.
* Validator was updated to allow resolved problems to appear as part of the Past Illness Section.

#### V 3.1.13 |   Released on: 3/26/2018

#### C-CDA Validator Updates:
* C-CDA Validator was updated to remove Encounter Diagnosis validation errors from View, Download, Transmit criteria.
* Updated RelationshipType value set for CarePlan documents.

#### FHIR Sandbox updates:
* Updated Google Analytics for FHIR Sandbox
* Updated Bulk FHIR API Server and deployed Beta Version.

#### V 3.1.12 |   Released on: 2/26/2018

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

#### V 3.1.11 |   Released on: 1/29/2018

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Add button with link to ONC One Click Scorecard page
* Added ccdaVersion and service errors for invalid formats

##### C-CDA Validator Updates: 
* Added ccda file name of the submitted file for debugging.
* Added warning messages for telecom content validation.


#### V 3.1.10 |   Released on: 11/30/2017

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

#### V 3.1.9  |   Released on: 10/30/2017

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

#### V 3.1.8  |   Released on: 9/26/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected One Click Scorecard Report Schema errors display to use proper sentence.

##### C-CDA Validator Updates: 
* The C-CDA Validator was updated to 1.0.23 with the following fixes.
* Updated the 170.315(b)(2) - CIRI Validation for R1.1 files which was missing. Prior to the release, the R1.1 file reconciliation output submitted to the validator was not being validated for content. This was updated to ensure content matching was performed with the R1.1 reconciliation file outputs. So if the reconciliation of R1.1 files does not produce the output following the instructions provided for the criteria, there will be errors displayed by the validator.
* Existing Smoking status validation bug was fixed which was previously preventing an error being displayed when smoking status entry was nullFlavored or missing. The fixing of the bug displays an error if smoking status does not include the proper test data provided.
* DS4P Validation was updated such that PurposeOfUseSecurityObservation/value and all other values and codes of templates which inherit from SecurityObservation now override their parent requirements. This allows for both templates to exist, but only the child's requirement to be enforced. This resolves the possible conflict of differing terminology requirements between a parent and child template. As a result, PurposeOfUseSecurityObservation value/@codesystem now requires ActReason 2.16.840.1.113883.5.8 as opposed to the prior requirement of ObservationValue 2.16.840.1.113883.5.1063, due to an error in the HL7 example XML.

##### FHIR Sandbox Updates: 
* Updated and fixed DSTU2 and STU3 validation for FHIR Tools.
* Fixed OAuth issues incluing password encryption, state parameter validation, removing cached authorization.

##### Direct Transport Sandbox Updates: 
* Added capability of using Interop@direct.hhs.gov for Direct Trust Users 


#### V 3.1.7  |   Released on: 8/29/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected Rubrics for Timestamp handling of Problems and Allergy Concern acts
* Corrected Rubrics for Narrative Text linking.
* Posted Rubrics document to the Website.

##### C-CDA Validator Updates: 
* Fixed DS4P validation to align with the DS4P IG and the Consent Directive IG.
* Fixed CCDS Content Validation for UDIs

##### FHIR Sandbox Updates: 
* Updated and fixed DSTU2 validation loging for DSTU2 FHIR Sandbox.


#### V 3.1.6  |   Released on: 8/1/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected issues with Date of Death Rubric timestamp validation.
* Added Rubric for Substance Administration Sig validation.
* Corrected issues with data encoding and handling UTF-8.

##### C-CDA Validator Updates: 
* Fixed DS4P validation to kick in correctly based on objectives.
* Updated Reference Validator to use 20170725 MDHT build and 20170707 DS4P build

##### FHIR Sandbox Updates: 
* Fixed error handling of Queries.
* Made text changes to remove Alpha Release, Run US Core Tests, Public client, Confidential client.
* Added Validation for STU3 Server in FHIR Query Tool.
* Added initial validation for DSTU2 Server responses in FHIR Query Tool.
* Updated data to trim white spaces for various FHIR data elements.


#### V 3.1.5  |   Released on: 6/26/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
* Corrected issues with Date of Birth Rubric timestamp validation.
* Corrected defects with lifespan validation rubric when observations occured at the same time as patient's death.
* Added rubric for Birth Sex Validation.
* Added rubric for Patient's Alternative Name Validation.
* Updated Metrics collection APIs to segregate One-Click Scorecard and UI.
* Updated Metrics to collect section based scoring, document based scoring.
* Changed Error Sample of Scorecard to get a C instead of A-.
* Updated HL7 Templates to include DS4P Templates.

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

#### V 3.1.4  |   Released on: 6/1/2017

##### C-CDA Scorecard / One-Click Scorecard Updates: 
- The C-CDA Scorecard was updated with the following changes:
* Removed industry averages from the Scorecard Report generated by the SITE UI.
* Added One-Click Scorecard links to Direct and C-CDA Sandboxes.

##### FHIR Sandbox Updates: 
* Supported DSTU2 and STU3 resources according to US Core Implementation Guide.
* Added missing queries to DSTU2 and STU3 Servers. 

##### C-CDA Validator Updates: 
* Fixed Immunization Value Set in MDHT.
* Accepted Code Modifications from the community for Code-Validator.
- Changed 2015 Certification Test Data to accomplish the following
* Made Document Ids across all the samples to make them unique.
* Updated RxNorm Codes in R11 Samples to use prescribable drugs.
* Updated Care Plan documents to include US Realm Header and R11 Section/Entry Template Ids.
* Fixed Language Code for Care Plan Samples.

#### V 3.1.3.1  |   Released on: 5/8/2017

##### C-CDA Scorecard Updates: 
- The C-CDA Scorecard was updated with the following changes:
* Fixed defects related to display name validation for code systems that do not exist in the vocabulary database.
* Fixed effective time handling related to patient lifespan when there is a nullFlavor for any of the times being compared. 
* Fixed effective time handling when there are just a single timestamp value vs a low and high for comparison with other time intervals.

##### FHIR Sandbox Updates: 
* Corrected defects which was preventing the Observation related profiles from returning data.
* Corrected defects to remove scopes from open server screens.
* Added additional missing US Core profiles in the Query Tool.

#### V 3.1.3  |   Released on: 4/25/2017

##### C-CDA Validator Updates: 
- The C-CDA validator was updated with the following changes:
* Fixed defects related to the Content Validation for Care Plan criteria (b)(9), CIRI criteria (b)(2) and DS4P criteria (b)(7).
* The defects were not validating the patient names correctly, the data in the document sections as needed for the criteria.

##### FHIR Sandbox Updates: 
* Updated FHIR Sandbox with to support STU3 server.
* Updated FHIR Sandbox to add validation service for future integration with conformance tool.

#### V 3.1.2  |   Released on: 3/28/2017

##### C-CDA Validator Updates: 

- The C-CDA validator was updated with the following changes:
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
- Defect Fixes
* Remove 'Detailed Results' header in saved PDF if there are no results
* Fix code system check for Null Pointer Exception.

##### FHIR Sandbox Updates: 
* Updated FHIR Sandbox with Medication Data Set from ONC MedList project.
* Updated FHIR Server Capabiltiy Statement (Conformance Statement) for STU2 version.
* Updated FHIR Server to support all Argonaut queries.

##### SITE UI Improvements:
* XDR Test Tool updated with the new UI themes, headers and footers.

#### V 3.1.1  |   Released on: 2/28/2017

##### C-CDA Validator Updates: 

- The 2015 Edition C-CDA Validator has been updated to Release 1.0.14 with the following changes.
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


#### V 3.1.0.1  |   Released on: 2/16/2017

##### C-CDA Validator Updates:

- The 2015 Edition C-CDA Validator has been updated to Release 1.0.12 with the following changes. 
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

- The Scorecard was updated with the following changes 
* The One-Click Scorecard for HIMSS 2017 was configured.
* The PDF Report was updated to have a summary and a interpretation guide.
* The Scorecard Display Name Validation was updated to leverage all the possible names in the vocabulary.
* The Conformance Errors were seperated from Certification Feedback.
* Updated Effective Time Element handling of partial times.
* Updated scoring logic to account for missing sections.
* Updated scoring rule for Lab Result validation and Vital Signs validation to look for PQ data type and enforce UCUM rules.
* Updated scoring rule for top 2000 LOINC codes. 
* The detailed Scorecard release notes can be accessed at ( https://github.com/onc-healthit/SITE-Content/blob/master/CCDAScorecardReleaseNotes.md ) 

#### V 3.1.0  |   Released on: 1/31/2017

##### C-CDA Validator Updates:

- The 2015 Edition C-CDA Validator has been updated to Release 1.0.11 with the following changes. 
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
*	Updated Scoring criteria to not apply rules to No Information or Null Sections which have no data or are completely absent
*	Updated Try Me to support multiple files (a high and low scoring sample and a sample with errors) and provided new and updated data
*	Updated top level results and summary UI layout
*	Added ability to identify 2015 Edition Certification Feedback and Empty Sections in the heatmap
*	For clarity, converted rubric sub-Description data ('Issues' and 'Best Practice') into tabs versus links
*	Embolden heat map text by default and hover attributes so that categories are both easier to read upfront and understand the status of overall
*	Added disabled option to the heatmap when categories have no issues to navigate to or are empty sections
*	Updated Conformance and Certification section to display a related issue count in brackets
*	Updated heatmap to jump to Certification or Conformance when a section has related issues versus jumping to a no-issue scorecard result
* Categories (including Conformance and Certification) which have no issues are no longer shown in the detailed results which allows for a cleaner, more focused interface
*	Updated IG/Cert. links to navigate via their label versus error count alone
* Added C-CDA Document Type (e.g. CCD) scored
* Each rubrics 'Issues' tab is now selected/expanded by default
* Replaced loading text with animations
* Reworded and moved 'Standard' option text to the end of each rubrics description versus in its own tab
* Updated to not load 'Detailed Results' button on a full pass scenario (100/100)
* Added 'Edition' to 2015 Certification Feedback
*	Updated color schemes
 	- 3 colors only (green, yellow, red) for all grade results
  - Category headers black versus blue to match heatmap
  - Cert and IG black in heatmap and detailed results
  
###### Fixes
*	Fixed heatmap category click/IG and Cert. links not opening detailed results if closed
*	Fixed issue where a C-CDA IG Conformance Error could be identified as a 2015 Edition Certification Feedback issue in the heatmap
* Fixed typos in a few locations


#### V 3.0     - 12/20/2016

- Updated CCDA Validator with the following fixes
* Relaxed the timing information validation for Problems, Medications, Allergies.
* Updated new MDHT Release which includes the following ERRATA for C-CDA R2.1 (710, 806, 808, 872, 986, 1018, 1220)
- Scorecard fixes and enhancements
 * Added the ability to score multiple C-CDA files
 * toggle IG Conformance/Certification results
 * improved proecessing time
- New SITE UI released
- Updated FHIR Sandbox with bug fixes idenified by ONC Testing.

#### V 2.4     - 11/30/2016
- Updated Reference C-CDA Validator to fix content validation for Labs/Vitals/Procedures/Immunizations.
- Upated FHIR Sandbox to fix error handling and displaying appropriate error messages and editing of clients.
- Updated Scorecard to incorporate feedback from Internal ONC team on decoupling the various validations and its results.
- The new SITE UI Makeover Release has been updated to have the ONC Tech Lab Themes and Layouts.

#### v.2.3.9   -10/31/2016
- Updated C-CDA Validator to version 1.0.5
- Updated FHIR Sandbox with bug fixes based on feedback and comments on Alpha Release.
- Updated DS4P Test Data PDF and Test XML files.
- Provided the new SITE UI Re-design concept.

#### v.2.3.8   -09/26/2016
- Updated SITE Scorecard URL.
- Deployed Alpha Release of SITE FHIR Sandbox.
- Deployed Alpha Release of SITE DS4P Validator.
- Deployed Updates to C-CDA Validator which includes test data, test xml files, vocabularies and HL7 errata.

#### v.2.3.7   -09/09/2016
- Added 'Try Me' Feature.
- Improved Error Handling and User Notification.
- Updated UI.
- Fix for Effective Time validation when present in seconds format. 

#### v.2.3.6.2 -08/19/2016   
- Addition of Unique Instance Identifier rule in SCORECARD under Miscellaneous Section.
- IG References for issues change dynamically based on type of document processed(R1.1, R2.1).

#### v.2.3.6.1 -08/09/2016
- Fixed time validation routine to not reduce scores when additional precision is specified as part of the time element.

#### v.2.3.6   -08/05/2016
- File contents are no longer encoded.
- File contents are sent as an attachment in using optimized XOP message.
- Full and minimial messages are sent correctly when selected from dropdown.

#### v.2.3.5 - 08/05/2016
- Added ability to save the scorecard results to PDF.
- Added context to IG References to Standards.
- Added HL7 Example Task Force links to Best Practice links.
- Scoring for documents is optimized in case of any section is null flavor.
- Updated vital sign UCUM validation to validate against its value set.
 
#### v.2.3.4 - 08/04/2016
- C-CDA Validator Update
- Latest MDHT build.
- LOINC displayname validation is now done against the LONG_COMMON_NAME rather than COMPONENT.
- Vocabulary bug fixes.
- C-CDA IG validation bug fixes.
- Reference Content validation bug fixes.
 
#### v.2.3.3   - 07/15/2016
- Added full support for C-CDA R1 to Scorecard - The Scorecard now fully supports scoring of documents that conform to either the  C-CDA R1.1 or the C-CDA R2.1 Implementation Guide.

#### v.2.3.2.1 - 07/08/2016
- Applied Scorecard hotfix - Fixed null flavor with problem status code throwing service error

#### v.2.3.2 - 06/28/2016
- Updated Reference C-CDA Validator - Updated Reference Validator to display content errors based on certification test data scenarios

#### 2.3.1 - 06/28/2016
- ONC C-CDA Scorecard (Beta) release
- Added Calculation of Industry Average (based on average of all scores since scorecard was made available)
- Updated method of counting issues discovered
- Enhancements for scoring both C-CDA R2.1 and R1.1 documents 
- Enhancements to section heatmap 

#### 2.3.0.1 - 06/08/2016
- Scorecard Hot fix for CDN/Broken link Issue

#### v.2.3.0 - 5/16/16
- C-CDA Validator Service Release
  * Fixed concurrency issue
  * Updated valuesets and validator configuration
- C-CDA Validator Portlet
  * 508 compliancy work
- Direct Transport Portlet
  * Addressed issues where x.509 certificates were being improperly loaded
- C-CDA Scorecard initial release

#### v.2.2.7 - 4/8/16
- C-CDA Validator Service Release
  * Problem Observation Valuesets
  * Vocabulary validation severity can be configured to be SHALL, SHOULD, MAY severity
  * CDT Codesystem is loaded but not yet configured
  * New MDHT Build

#### v.2.2.6 - 2/29/16
- C-CDA Validator Service Release
  * Improved validation performance, most validations should take under 1 minute.
- XDR Validator Service Release
  * Responses are now in MTOM format
  * Fixed where some nodes were not found due to incorrect Qnames.

#### v.2.2.5 - 1/31/16
- New MDHT Release for IG conformance
- Vocabulary Updates to include Non-VSAC value sets
- Reference CCDA IG updates
- Test Data updates for C-CDA certification criteria

#### v.2.2.4 - 12/23/2015
- C-CDA Validator Release
- MDHT Update
- UI Update
- Added Test Data Repository

#### v.2.2.3 - 12/09/2015
- Upgraded C-CDA 2.1 Validator
- Deployed new C-CDA valuesets and updated configuration(s)
- Extended validator and Reference validator with separate R1 and R2 configurations
- Updated validators and valueset/codes to enable configuration for path expression
- Added DVT FAQs
- Added 2015 DCDT
- Updated Direct Sandbox Links

#### v2.2.2 - 10/30/2015
- Upgraded SITE C-CDA Validator
  * Added the Reference C-CDA Validator functionality for R2.0
  * Added vocabulary valueset validation for new code system files
  * Added vocabulary valueset validation for new value sets available from VSAC

#### v2.2.1 - 09/27/2015
- Upgraded SITE C-CDA Validator from R2.0 to R2.1
- Retired SITE QRDA Validator

#### v2.2.0 - 08/17/2015
- Added finalized 508 Compliance UX
- Added Vocabulary Validation to the C-CDA Validator
- New version of SITE Direct Transport Standard Testing Services (1.1)
- New C-CDA R1.1 and R2.0 builds
       
#### v2.1.0 - 07/10/2015
- Added the SITE Direct Transport Standard Testing Services

#### v2.0.4 - 05/01/2015
- Updated Virtual Machines to fix the GHOST flaw
- Increase VM disk size

#### v2.0.3 - 04/30/2015
- Added the CYPRESS QRDA Validator to the Quality Reporting Standard Sandbox and Testing Resources Pages

#### v2.0.2 - 04/17/2015
- Added the SITE Direct SMTP Edge Test Tool
- Added optional parameters to the SITE Direct XDR Edge Test Tool
- Fixed issues in formatting of a Provider Directory response
- Completed additional required Section 508 Accessibility Issues
- Added Bonnie to the CQM Sandbox
- Added Public Health Reporting, Laboratory Standards, Electronic Prescribing, and SOAP Transport Sandboxes

#### v2.0.1 - 02/26/2015
- Added the SITE Direct XDR Edge Test Tool

#### v2.0 - 12/31/2014
- Refactored all of the SITE portlet code
- Updated SITE C-CDA Validator to version 2.0
- Updated SITE Direct Transport Test Tool to version 2.0
- Updated SITE Provider Directory Test Tool to version 2.0
- Updated SITE QRDA Validator to version 2.0

#### v1.3.9 - 12/26/2014
- Updated SITE Provider Directory Test Tool to version 1.1

#### v1.3.8 - 11/11/2014
- Incorporated the CQM Certification Sandbox
- Updated look and feel of the SITE application

#### v1.3.7 - 10/01/2014
- Incorporated the Direct Certificate Discovery Tool

#### v1.3.6 - 07/30/2014
- Updated the look and feel of SITE to support Section 508 Compliance

#### v1.3.5 - 07/18/2014
- Updated the C-CDA validation service (new MDHT build)

#### v1.3.4 - 07/10/2014
- Incorporated SITE Statistics for existing portlets

#### v1.3.3 - 06/13/2014
- Updated C-CDA Validator to version 1.5

#### v1.3.2 - 05/01/2014
- Updated SITE to address the potential Heartbleed issue.

#### v1.3.1 - 04/08/2014
- Addressed defects in both the Provider Directory Test Tool and the QRDA Validator

#### v1.3 - 03/06/2014
- SITE Usability Updates

#### v1.2 - 01/28/2013
- Addition of Federated HPD and QRDA sandboxes

#### v1.1 - 06/30/2013
- Addition of the Direct Sandbox

#### v1.0 - 04/09/2013
- Addition of the C-CDA Sandbox

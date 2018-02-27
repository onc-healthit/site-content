# The Standards Testing & Implementation Environment (SITE)
## Release Notes

#### V 3.1.12 |   Released on: 2/26/2018

#### C-CDA Validator Updates:
* C-CDA Validator was updated to produce warnings for care plan sections that are mentioned in the test data but are a SHOULD in the IG.
* Updated IG validation to align MedicationSection/code rules with R1.1 C-CDATemplateLibrary.

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
* System messages will display under the banner when the SITESystemMessage markdown has content. ( https://github.com/siteadmin/SITE-Content/blob/master/SITESystemMessage.md )
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
* The detailed Scorecard release notes can be accessed at ( https://github.com/siteadmin/SITE-Content/blob/master/CCDAScorecardReleaseNotes.md ) 

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
- Addition of the C-CDA Sanbox

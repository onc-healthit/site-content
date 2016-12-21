# The Standards Testing & Implementation Environment (SITE)
## Release Notes

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

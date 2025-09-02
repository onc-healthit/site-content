**SITE Platform Version: 4.1.7 | Released on 8/29/2025**
 
**Versions and Changes to various Components in the Release 4.1.7**
 
 
| Component                                      | Version | Updated in Release |
|:————————————————————————-----------------------|:—---———:|———---------———————:|
| C-CDA Certifiation Test Data                   | 1.1.1   | Yes                |
| C-CDA Code Validator API                       | 1.0.3   | No                 |
| C-CDA Content Validator API                    | 1.1.4   | Yes                |
| C-CDA Reference Validator API                  | 1.1.3   | Yes                |
| Edge Test Tool (Direct/Direct Edge Protoocols) | 2.3.74  | No                 |
| SITE User Interface (site-ui-4)                | 4.1.6   | No                 |
| XDR Message Validator                          | 1.0.2   | No                 |
| XDR Message Sender                             | 1.0.3   | No                 |
| Trust Anchor Uploader                          | 1.0.1   | No                 |
| Direct Certificate Discovery Tool (DCDT)       | 3.1.7   | Yes                |
| Direct Transport Message Sender                | 1.0.3   | No                 |
| C-CDA Scorecard                                | 2.7.2   | No                 |
 
 
**C-CDA Certification Test Data Changes:**
 
For USCDIv3 and USCDIv4 test data : 
170.315(b)(1) Transitions of Care, 170.315(e)(1) VDT, 170.315(g)(9) API Access criteria Inpatient and Ambulatory Criteria:
 
Updates in Sample 3:
 - Removed sdtc:raceCode requirement
 - Changed Happy Kid Sex to Female
 - Updated Related Person Frank Larson to relationship of type Father 
 
Updates in Sample 1: 
 - Removed unit requirement for Specific Gravity
 - Clarified Payer Id root value needs to be present but any value can be used 
 - Added Specimen Type data element 
 
 
**C-CDA Content Validator API Changes: Updates to Validation**
 - Updated Validator to check for null pointer when printing Assessments
 - Downgraded sdtc:raceCode to WARNING instead of ERROR 
 - Updated Procedure Validations to account for test data present in code.translation element
 - Updated Functional Status validation to enforce Disability Status and Functional Status Observations in content validation
 - Updated Document Template validation for USCDIv3 to use US Realm Header with  2023-05-01 extension
 - Updated Validators to use either PQ or ST for Specific Gravity lab result
 
**SITE-UI Changes for Direct Sender/Receiver Message Status** 
 - Added download button to download the Direct Validation Report in CSV format for Outgoing Messages

# The Standards Testing & Implementation Environment (SITE)

## Release Notes

#### Our commitment to transparency and keeping you informed about the latest updates is at the heart of this section. Whether you're a developer, an IT professional, or a healthcare stakeholder, our release notes provide valuable insights into the evolution of our platform.

## Latest Release
### SITE Platform Version: 4.1.6 | Released on 7/29/2025

#### Versions and Changes to various Components in the Release 4.1.6 


| Component                                      | Version | Updated in Release |
|------------------------------------------------|---------|--------------------|
| C-CDA Certifiation Test Data                   | 1.1.1   | Yes                |
| C-CDA Code Validator API                       | 1.0.34  | No                 |
| C-CDA Content Validator API                    | 1.1.3   | Yes                |
| C-CDA Reference Validator API                  | 1.1.2   | Yes                |
| Edge Test Tool (Direct/Direct Edge Protoocols) | 2.3.74  | No                 |
| SITE User Interface (site-ui-4)                | 4.1.5   | No                 |
| XDR Message Validator                          | 1.0.2   | No                 |
| XDR Message Sender                             | 1.0.3   | No                 |
| Trust Anchor Uploader                          | 1.0.1   | No                 |
| Direct Certificate Discovery Tool (DCDT)       | 3.1.7   | Yes                |
| Direct Transport Message Sender                | 1.0.3   | No                 |
| C-CDA Scorecard                                | 2.7.2   | No                 |

#### C-CDA Certification Test Data Changes:
 
For USCDIv3 and USCDIv4 test data :
170.315(b)(1) Transitions of Care, 170.315(e)(1) VDT, 170.315(g)(9) API Access criteria:

Updates in Ambulatory Sample 1:
* Removed Gender Identity data element
* Removed Sexual Orientation data element
* Removed Health Insurance Type Data Element from Coverage Type to be in sync with ERRATA and US Core and removed translation value.
* Changed Payer Root Identifier to 2.16.840.1.113883.6.300 reflecting NAICS OID
* Updated guidance for Group Identifier root to be optional and can be changed by vendors
* Updated SDOH Goal Achieve By Date to be Optional

Updates in Ambulatory Sample 2
* Removed Gender Identity data element
* Removed Sexual Orientation data element

Updates in Inpatient Sample 1:
* Removed Gender Identity data element
* Removed Sexual Orientation data element
* Removed Health Insurance Type Data Element from Coverage Type to be in sync with ERRATA and US Core and removed translation value.
* Changed Payer Root Identifier to 2.16.840.1.113883.6.300 reflecting NAICS OID
* Updated guidance for Group Identifier root to be optional and can be changed by vendors
* Updated SDOH Goal Achieve By Date to be Optional

Updates to USCDIv1
* Changed CIRI R11 Sample to use the right allergy severity of Mild instead of “Mild to Moderate”

#### C-CDA Content Validator API Changes: Updates to Validation
* Removed Effective Time Validation for Procedure Activity Procedure
* Updated Gender Value Set to be dynamic instead of Static in MDHT
 
#### DCDT Changes
* Updated DCDT DNS Certificates CRL URL to function without a 404 error


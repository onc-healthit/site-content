# The Standards Testing & Implementation Environment (SITE)

## Release Notes

#### Our commitment to transparency and keeping you informed about the latest updates is at the heart of this section. Whether you're a developer, an IT professional, or a healthcare stakeholder, our release notes provide valuable insights into the evolution of our platform.

## Latest Release
### 4.1.6 | Released on 7/29/2025

#### C-CDA Changes:
 
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

Updates to Validation
* Removed Effective Time Validation for Procedure Activity Procedure
* Updated Gender Value Set to be dynamic instead of Static in MDHT
 
#### DCDT Changes
* Updated DCDT DNS Certificates CRL URL to function without a 404 error


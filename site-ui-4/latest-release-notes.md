# The Standards Testing & Implementation Environment (SITE)

## Release Notes

#### Our commitment to transparency and keeping you informed about the latest updates is at the heart of this section. Whether you're a developer, an IT professional, or a healthcare stakeholder, our release notes provide valuable insights into the evolution of our platform.

## Latest Release
### 4.1.5 | Released on 6/23/2025
* [SITE User Interface 4](https://github.com/onc-healthit/site-ui-4) updated to version [4.1.5](https://github.com/onc-healthit/site-ui-4/releases/tag/4.1.5)
	* Update document selection in direct tooling for b1, h1, and h2 from "Cures" and "SVAP" to "USCDIv1", "USCDIv3", and "USCDIv4". (SITE-4597)
	* Fix index display bug not showing new notifications. (SITE-4634)
	* Add new notification: XDR SMTP updates. (SITE-4634)
	* Fix "invalid digest" toggle when sending direct message. (SITE-4532)
	* Fix XDR Test 5 message not sending a document. (SITE-4643)
* [Edge Testing Tool](https://github.com/onc-healthit/ett) updated to version [2.3.74](https://github.com/onc-healthit/ett/releases/tag/2.3.74)
	* Update document selection in direct tooling for b1, h1, and h2 from "Cures" and "SVAP" to "USCDIv1", "USCDIv3", and "USCDIv4". (SITE-4597)
	* Generate Direct Validation Report email URL for SITE UI 4. (SITE-4554)
* [Content Validator API](https://github.com/onc-healthit/content-validator-api) updated to version [1.1.2](https://github.com/onc-healthit/content-validator-api/releases/tag/1.1.2)
	* Update procedure activity procedure entry effective time comparison to use either value or low/high value. (SITE-4567)
	* Update planned procedure comparison to check both "plan of treatment" and "assessment and plan" sections. (SITE-4555)
* [Direct Certificate Discovery Tool](https://github.com/onc-healthit/dcdt) updated to version [3.1.6](https://github.com/onc-healthit/dcdt/releases/tag/3.1.6)
	* Fix for issue related to mismatch of Authority Key identifier of the leaf certificate to the Subject Key Identifier of the root certificate. (SITE-4551, SITE-4553, SITE-4561)

* The following components are used in this version of SITE. Components marked with * were updated with this release.
	* [C-CDA Scorecard 2.7.2](https://github.com/onc-healthit/ccda-scorecard/releases/tag/2.7.2)
	* [C-CDA USCDI Certification Test 1.1.0](https://github.com/onc-healthit/ccda-uscdi-certification-testdata/releases/tag/1.1.0)
	* [Code Validator API 1.0.34](https://github.com/onc-healthit/code-validator-api/releases/tag/1.0.34)
	* [Content Validator API 1.1.2](https://github.com/onc-healthit/content-validator-api/releases/tag/1.1.2)*
	* [Direct Certificate Discovery Tool 3.1.6](https://github.com/onc-healthit/dcdt/releases/tag/3.1.6)*
	* [Direct Transport Message Sender 1.0.3](https://github.com/onc-healthit/direct-transport-message-sender/releases/tag/1.0.3)
	* [Edge Testing Tool 2.3.74](https://github.com/onc-healthit/ett/releases/tag/2.3.74)*
	* [Reference C-CDA Validator 1.1.1](https://github.com/onc-healthit/reference-ccda-validator/releases/tag/1.1.1)*
	* [SITE Content 4.1.5](https://github.com/onc-healthit/site-content/releases/tag/4.1.5)*
	* [SITE User Interface 4 4.1.5](https://github.com/onc-healthit/site-ui-4/releases/tag/4.1.5)*
	* [Trust Anchor Uploader 1.0.1](https://github.com/onc-healthit/trustanchor-uploader/releases/tag/1.0.1)
	* [XDR Message Sender 1.0.3](https://github.com/onc-healthit/xdr-message-sender/releases/tag/1.0.3)
	* [XDR Message Validator 1.0.2](https://github.com/onc-healthit/xdr-message-validator/releases/tag/1.0.2)

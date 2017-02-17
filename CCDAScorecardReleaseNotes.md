#### Release Notes

* Updates included in the **SITE 3.1.0.1 02/16/2017 Release** for the **C-CDA Scorecard 'HIMSS 2017'**

  * Improvements
    * Added a new web service at endpoint savescorecardservicebackendsummary which drives the "One Click" scorecard for use with Direct by providing a comprehensive PDF report response
      * This differs from the savescorecardservicebackend service in that it has its own specific format of the results (A summary, a dynamic results table, a static guide table with 'call outs', and a detailed key)
    * Updated the Scorecard website to be consistent with the 2017 SITE UI
    * Updated the Scorecard website to handle dynamic SITE content
    * Removed IG-based results from 2015 Edition Certification Feedback results
    * Updated 'Try Me' data (JSON) for all 3 samples and XML for the high scoring sample
    * Added links with resources to some rule descriptions for help with best-practices, for example, the top 2000 LOINC codes for a related Lab Results issue
    * Updated the save PDF report to incorporate conformance errors, certification errors, null, or empty results, per section
      * Allows the report to display messages like:
       * "This category was not scored as it is an empty section"
       * "This category was not scored as it contains Certification Feedback"
       * "This category was not scored as it contains Conformance Errors"
    * Updated the save PDF report to not show or link to categories without issues and to include links to IG/Cert issues from the heatmap
    * Updated all PDF services to use the latest HealthIt.gov SITE header
    * Updated various rubric messages
  
  * Fixes
    * Missing sections are now treated the same as null flavor sections
    * Updated handling of effectiveTime element values
    * Changed handling of templateId rule validation to consider only the IDs in the C-CDA IG
    * Updated effectiveTime/@value rules to not reduce score when positive offsets are specified
    * Updated HITSP Vital Sign result set to include additional values
    

#### Release Notes

* Updates included in the **SITE 3.1.0. 1/30/2017 Release** for the **C-CDA Scorecard 'Beta 3'**

  * Improvements
    1.  Updated Effective Date Time Rule to handle partial dates/times
    2.  Updated Unique Id rule to not apply on the header participants such as Author
    3.  Updated Display Name rule to not apply when display names are not present
    4.  Updated Text Reference Checking Rule to account for sub elements in tables in the narrative text
    5.  Updated Scoring criteria to not apply rules to No Information or Null Sections which have no data or are completely absent
    6.  Updated Try Me to support multiple files (a high and low scoring sample and a sample with errors) and provided new and updated data
    7.  Updated top level results and summary UI layout
    8.  Added ability to identify 2015 Edition Certification Feedback and Empty Sections in the heatmap
    9.  For clarity, converted rubric sub-Description data ('Issues' and 'Best Practice') into tabs versus links
    10.  Embolden heat map text by default and hover attributes so that categories are both easier to read upfront and understand the status of overall
    11.  Added disabled option to the heatmap when categories have no issues to navigate to or are empty sections
    12.  Updated Conformance and Certification section to display a related issue count in brackets
    13.  Updated heatmap to jump to Certification or Conformance when a section has related issues versus jumping to a no-issue scorecard result
    14.  Categories (including Conformance and Certification) which have no issues are no longer shown in the detailed results which allows for a cleaner, more focused interface
    15.  Updated IG/Cert. links to navigate via their label versus error count alone
    16.  Added C-CDA Document Type (e.g. CCD) scored
    17.  Each rubrics 'Issues' tab is now selected/expanded by default
    18.  Replaced loading text with animations
    19.  Reworded and moved 'Standard' option text to the end of each rubrics description versus in its own tab
    20.  Updated to not load 'Detailed Results' button on a full pass scenario (100/100)
    21.  Added 'Edition' to 2015 Certification Feedback
    22.  Updated color schemes
        * 3 colors only (green, yellow, red) for all grade results
        * Category headers black versus blue to match heatmap
        * Cert and IG black in heatmap and detailed results
  
  * Fixes
    1.  Fixed heatmap category click/IG and Cert. links not opening detailed results if closed
    2.  Fixed issue where a C-CDA IG Conformance Error could be identified as a 2015 Edition Certification Feedback issue in the heatmap
    3.  Fixed typos
    

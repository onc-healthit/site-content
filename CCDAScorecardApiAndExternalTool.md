#### Scorecard External Tool Instructions

*   **How to Use the Scorecard Batch Application:**
    *   Either download the instructions [here](https://github.com/onc-healthit/scorecard-batch/raw/master/artifacts/Scorecard-%20Batch-%20Process-Instructions.docx) or read the following instructions:
        1.  Download the jar file from [https://github.com/onc-healthit/scorecard-batch/tree/master/artifacts](https://github.com/onc-healthit/scorecard-batch/tree/master/artifacts)

        2.  Please create the config file scorecard-batch.config with the following properties:

            *   scorecardBatch.ccdaFileLocation=/var/opt/scorecard/ccdaFiles

            *   scorecardBatch.outputFolderLocation=

            *   scorecardBatch.scorecardUrl=https://devccda.sitenv.org/scorecard/ccdascorecardservice2

            A sample config file can be found at [https://github.com/onc-healthit/scorecard-batch/blob/master/src/main/resources/scorecard-batch.config](https://github.com/onc-healthit/scorecard-batch/blob/master/src/main/resources/scorecard-batch.config)

            *   **scorecardBatch.ccdaFileLocation** - Folder location where all the CCDAs are placed for scoring. This is a mandatory property

            *   **scorecardBatch.outputFolderLocation** - Folder location to save the response files. If this is not specified a default folder scorecardBatchOutput is created in root folder and are saved to this location

            *   **scorecardBatch.scorecardUrl** - Specify the scorecard service end point for response. If this is not specified, the batch process will default to the Scorecard Production Server Endpoint

        1.  **Open Command Prompt and Run As Administrator**. Navigate to the location where the jar file is placed. For example, the jar file is placed under C:\Projects

            Execute the following command:
            
            ```bash
            java -DconfigFileLocation="C:/var/opt/scorecard/scorecard-batch.config" -jar scorecard-batch.jar
            ```

        1.  The response files will be created in the folder specified in the location specified in the **scorecardBatch.outputFolderLocation** property of the config file

# automation_for_ur_at_scale
Code presented during my talk @ Spotify (February 2020). Scripts and example to embed user data into a Qualtrics survey and create clean, interpretable, data exports.

To try the example:
1. Import `survey.qsf` into Qualtrics (click here to learn how to import a survey)[https://www.qualtrics.com/support/survey-platform/survey-module/survey-tools/import-and-export-surveys/#ImportingASurvey]

2. Open `embed_user_data_into_survey.ipynb` in Jupyter Notebooks. Before running through any code you'll need to:
  - Enter your Qualtrics IDs (click here to learn how to find your Qualtrics IDs)[https://www.qualtrics.com/support/integrations/api-integration/finding-qualtrics-ids/#LocatingQualtricsIDs]
  - Ensure that you have access to the Qualtrics API; otherwise you'll get response code 403 when you try to embed the variable headers and it will not work. I had to contact my IT administrator in order to receive access.
  
3. Create some fake data! Go to the data folder and open `survey_distribution_list.xlsx`. Click on a few of the links and fill out the survey to generate data.

4. Open `export_survey_data.ipynb` in Jupyter Notebooks. Before running through the code, make sure to enter your Qualtrics IDs (click here to learn how to find your Qualtrics IDs)[https://www.qualtrics.com/support/integrations/api-integration/finding-qualtrics-ids/#LocatingQualtricsIDs].

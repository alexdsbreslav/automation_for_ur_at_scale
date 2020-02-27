# Automation for UR at Scale
Code presented during my talk @ Spotify (February 2020). I have included the survey and scripts used in the example so that anyone interested could try it themselves. The scripts interact with the Qualtrics API to:
    - Make embedding user data into a Qualtrics survey efficient and reproducible
    - Create clean, and interpretable, data exports.

## To try the example:
1. Import `survey.qsf` into Qualtrics .
    - Once imported, make sure you hit the publish button.
    - Notice that all of the questions and response choices are labeled - this helps make the data exports much easier to read!

2. Open `embed_user_data_into_survey.ipynb` in Jupyter Notebooks. Before running through any code you'll need to:
    - Enter your Qualtrics IDs.
    - Ensure that you have access to the Qualtrics API; otherwise you'll get response code 403 when you try to embed the variable headers and it will not work. I had to contact my IT administrator in order to receive access.
  
3. Create some fake data! Go to the data folder and open `survey_distribution_list.xlsx`. Click on a few of the links and fill out the survey to generate data.

4. Open `export_survey_data.ipynb` in Jupyter Notebooks. Before running through the code, make sure to enter your Qualtrics IDs.

## Helpful links from Quatlrics:
- [How to import a survey from a QSF file.](https://www.qualtrics.com/support/survey-platform/survey-module/survey-tools/import-and-export-surveys/#ImportingASurvey)
- [How to publish your survey.](https://www.qualtrics.com/support/survey-platform/survey-module/survey-publishing-versions/#PublishingNew)
- [How to edit the question labels in Qualtrics.](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/formatting-questions/#EditingQuestionLabels)
- [How to edit the response choice labels in Qualtrics.](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/recode-values/#RecodingValuesAndChangingVariableLabels)
- [How to find your Qualtrics IDs.](https://www.qualtrics.com/support/integrations/api-integration/finding-qualtrics-ids/#LocatingQualtricsIDs)

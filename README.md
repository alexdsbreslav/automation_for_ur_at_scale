# Automation for UR at Scale
Code presented during my talk for the Product Insights team at Spotify (February 2020). I have included the survey and scripts used in the example so that anyone interested could try it themselves. The scripts interact with the Qualtrics API to: one, automatically embed user data into a Qualtrics survey, and two, automatically create clean and interpretable data exports.

## To try the example:
1. Download `survey.qsf` and import it into Qualtrics
    - Once imported, make sure you hit the publish button
    - Notice that all of the questions and response choices are labeled - this helps make the data exports much easier to read!

2. Open the Github repo. You can do this in two ways:
    - If you have Jupyter Notebooks on your computer: clone the repo and navigate to the scripts folder in Jupyter
    - If you do not have Jupyter Notebooks: click here &rarr; [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/alexdsbreslav/automation_for_ur_at_scale/master) to launch the code using a website called Binder. Binder will take a few minutes to load, but once it loads, you'll have everything you need to run the scripts!

3. Navigate to the scripts folder and open `embed_user_data_into_survey.ipynb`. Once you have the code open:
    - Enter your Qualtrics IDs.
    - Ensure that you have access to the Qualtrics API.
        - If you do not, you'll see `<Response 403>` when you try to embed the variable headers and it will not work. 
        - I had to contact my IT administrator in order to receive access.
  
4. Once you have created your embedded data fields using the code above, create some fake data!
    - Go to the data folder and open `survey_distribution_list.xlsx`. If you opened the code using Binder, download `survey_distribution_list.xlsx` and open it on your computer.
    - Click on a few of the links and fill out the survey to generate your fake data.

5. Navigate back to the scripts folder and open `export_survey_data.ipynb`. Before running through the code, make sure to enter your Qualtrics IDs.

## Helpful links from Qualtrics:
- [How to import a survey from a QSF file.](https://www.qualtrics.com/support/survey-platform/survey-module/survey-tools/import-and-export-surveys/#ImportingASurvey)
- [How to publish your survey.](https://www.qualtrics.com/support/survey-platform/survey-module/survey-publishing-versions/#PublishingNew)
- [How to edit the question labels in Qualtrics.](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/formatting-questions/#EditingQuestionLabels)
- [How to edit the response choice labels in Qualtrics.](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/recode-values/#RecodingValuesAndChangingVariableLabels)
- [How to find your Qualtrics IDs.](https://www.qualtrics.com/support/integrations/api-integration/finding-qualtrics-ids/#LocatingQualtricsIDs)

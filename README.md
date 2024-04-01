#### Bridget Sands
#### Harvard University
#### Applied Mathematics Senior Thesis
#### April 1st, 2024

## README.md: 
#### This serves as a guide to the files included in my SeniorThesis GitHub repository.

### In the general section of files:
- **data.zip**: zip file containing data used
  - Files under *data_from_R* output from *Data_Acquisition.Rmd* and input for *Clean_OB.ipynb*
  - Files under *data_cleaned_OB* output from *Clean_OB.ipynb* and input for *Data_Cleaning_PA.ipynb* and *Data_Cleaning_SB.ipynb*

- **Data_Aquisition.Rmd**: Provides code to access pbp data for all seasons
    - Output files stored within *data.zip*, in *data_from_R* folder

- **Clean_OB.Rmd**: Provides code to clean and adjust "Men_OB" feature of pbp data
  - Input files stored within *data.zip*, in *data_from_R* folder
  - Ouput files stored within *data.zip*, in *data_cleaned_OB* folder

- **ABS_teams.Rmd**: Provides code to acquire game_pks of Triple-A teams from 2022 season that used automated ball and strike system (ABS)
- **problem_pks.csv**: Output of *ABS_teams.Rmd*, list of game_pks of Triple-A games from 2022 in which ABS was active
    - Used as inputs for *Data_Cleaning_PA.ipynb* and *Data_Cleaning_SB.ipynb*

- **Data_Cleaning_PA.Rmd**: Provides code to clean and prepare data for final PA model
  - Main input files stored within *data.zip*, in *data_cleaned_OB* folder
  - Additional input file, *problem_pks.csv*
  - Ouput files stored within */PA/PA_data.zip*

- **Data_Cleaning_SB.Rmd**: Provides code to clean and prepare data for final SB model
  - Main input files stored within *data.zip*, in *data_cleaned_OB* folder
  - Additional input file, *problem_pks.csv*
  - Ouput files stored within */SB/SB_data.zip*

### In the PA folder:
- **PA_data.zip**: zip file containing data used
  - Files under *data_from_R* output from *Data_Cleaning_PA.ipynb* and input for *PA_model.Rmd*

- **Final_fitted_PA_models.zip**: zip file containing final fitted R model objects for overarching as well as count sub-models
  - Each sub-model has its own folder within it, containing:
      1) .txt output of the model summary
      2) The .rds model object
      3) A .csv file with output of fitted values
   
- **PA_model.Rmd**:
    - Used to fit the PA outcome models
  
### In the SB folder:
- **SB_data.zip**: zip file containing data used
  - Files under *data_from_R* output from *Data_Cleaning_SB.ipynb* and input for *SB_model.Rmd*

- **Final_fitted_SB_models.zip**: zip file containing final fitted R model objects for overarching as well as count sub-models
  - Each sub-model has its own folder within it, containing:
      1) .txt output of the model summary
      2) The .rds model object
      3) .txt output of the model summary for model fit without "AB_pickoffs" feature
      2) The .rds model object for model fit without "AB_pickoffs" feature
   
- **SB_model.Rmd**:
    - Used to fit the SB attempt models
  
### NOTE: I should have called all of the "SB" models "SBA" to be consistent with how I refer to it in my actual thesis. My mistake.








  

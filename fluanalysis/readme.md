# Readme.md File

Scripts used for (pre)processing/cleaning and analysis will be found in the "code" folder, and both raw and cleaned data is found in the "data" file.

## Code

### Wrangling

In the cleaning process, several columns and observations containing NA values are removed. For more information, please view the Quarto/R document.

### Exploration

Variables of interest explored through tables, violin graphs, and boxplots include Nausea (main categorical outcome), SwollenLymphNodes, ChillsSweats, SubjectiveFever, Headache, MyalgiaYN, Myalgia, EarPn, Vomit, and BodyTemp (Main Continuous Outcome). For more information, please view the Quarto/R document.

Predictors for Nausea are:

-   Headache

-   EarPn

-   Vomit

Predictors for BodyTemp are:

-   SwollenLymphNodes

-   SubjectiveFever

-   MyalgiaYN

-   Myalgia

-   ChillsSweats

### Model Fitting
Model fitting was accomplished through the `tidymodels` package (code saved) and re-evaluated using base R's *glm()* and *lm()* functions (code not saved).

## Data

### Raw Data

The raw data was obtained from <https://datadryad.org/stash/dataset/doi:10.5061/dryad.51c59zw4v> and saved as "SympAct_Any_Pos.Rda".

### Cleaned Data

The cleaned data is named as "cleaned_data.rds".

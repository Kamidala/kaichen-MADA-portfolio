# Readme.md File

Scripts used for (pre)processing/cleaning and analysis will be found in the "code" folder, and both raw and cleaned data is found in the "data" file.

## Code

### Wrangling

In the cleaning process, several columns and observations containing NA values are removed. After cleaning, the list of columns include: SwollenLymphNodes, ChestCongestion, ChillsSweats, NasalCongestion, CoughYN, Sneeze, Fatigue, Subjective Fever, Headache, Weakness, WeaknessYN, CoughIntensity, CoughYN2, Myalgia, MyalgiaYN, RunnyNose, AbPain, ChestPain, Diarrhea, EyePn, Insomnia, ItchyEye, Nausea, EarPn, Hearing, Pharyngitis, Breathless, ToothPn, Vision, Vomit, Wheeze, and BodyTemp. For more information, please view the Quarto/R document.

### Exploration

Variables of interest explored through tables, violin graphs, and boxplots include (among others) Nausea (main categorical outcome), SwollenLymphNodes, ChillsSweats, SubjectiveFever, Headache, MyalgiaYN, Myalgia, EarPn, Vomit, and BodyTemp (Main Continuous Outcome). For more information, please view the Quarto/R document.

Predictors of interest for Nausea in exploratory analysis are:

-   Headache

-   EarPn

-   Vomit

Predictors of interest for BodyTemp in exploratory analysis are:

-   SwollenLymphNodes

-   SubjectiveFever

-   MyalgiaYN

-   Myalgia

-   ChillsSweats

### Model Fitting
Model fitting was accomplished through the `tidymodels` package and re-evaluated using base R's *glm()* and *lm()* functions. BodyTemp acts as the main continuous outcome of interest, and Nausea acts as the main categorical outcome of interest. All other columns from the cleaned dataset will be treated as predictors. For more information, please view the Quarto/R document.

## Data

### Raw Data

The raw data was obtained from <https://datadryad.org/stash/dataset/doi:10.5061/dryad.51c59zw4v> and saved as "SympAct_Any_Pos.Rda".

### Cleaned Data

The cleaned data is named as "cleaned_data.rds".

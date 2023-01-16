# FIFA Quarto
We utilize Quarto to perform reproducible data analysis (with R), on Wage Prediction of [FIFA dataset](https://www.kaggle.com/datasets/stefanoleone992/fifa-22-complete-player-dataset) from 2018-2022.
To reproduce the analysis and generate the Quarto-based report, perform the following steps:

1. Clone the git repo using: 
```
git clone https://github.com/shyamshankarhr/fifa-quarto.git
```

2. Ensure that R is installed. Else, install it from https://cran.r-project.org/
   (To ensure complete reproducibility of the numbers as in the sample_result, use R version: 4.2.2 since the pseudorandom generators are different in different versions, and even seeding won't give consistent outputs (over different versions of R).

3. Install Quarto (if not done already). It is available [here](https://quarto.org/docs/get-started/).

4. In the cloned project directory, run the following command on command prompt:
```
quarto render FifaWage.qmd --to html
```
This may take around 20 minutes to run.

5. The report is generated as FifaWage.html

## Reproducibility

The report is not hard-coded, but generated based on the data files, and analysis results. The generated output file (FifaWage.html) will be similar to html report in sample_output folder (if the R-version is consistent). This shows the ability of Quarto to reproduce dynamic Data Analysis reports.
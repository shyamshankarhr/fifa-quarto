# FIFA Quarto
We utilize Quarto to perform reproducible data analysis (with R), on Wage Prediction of [FIFA dataset](https://www.kaggle.com/datasets/stefanoleone992/fifa-22-complete-player-dataset) from 2018-2022.
To reproduce the analysis and generate the Quarto-based report, perform the following steps:

1. Clone the git repo using: 
```
git clone https://github.com/shyamshankarhr/fifa-quarto.git
```

2. Ensure that R is installed. Else, install it from https://cran.r-project.org/

   Also ensure that the following r packages are installed:
      * dplyr
      * tidyverse
      * corrplot
      * randomForest
      * VIM
      * mice
      * kableExtra
      * MASS
      * MLmetrics
      * xgboost
      * fastDummies

3. Install Quarto (if not done already). It is available [here](https://quarto.org/docs/get-started/).

4. In the cloned project directory, run the following command on command prompt:
```
quarto render FifaWage.qmd --to html
```

5. The report is generated as FifaWage.html
# Healthcare Cost Modelling Project
This repo contains a project I am working on for my Data Science toolkit class.
The health_insurance.csv data set was downloaded from [Kaggle] (https://www.kaggle.com/raghupalem/insurance-charges) and it contains a cross-section of Health related variables for a sample of 1338 individuals.
For this project, the dependent variable would be Expenses.
I plan to build a model that uses other variables in the data set to predict potential yearly health expenses for a given patient.
Code would be written exclusively in R and a .R and .Rmd file

## Software Needed to Run Code

The following software and packages are needed to run code. Note that all packages are R packages
* R version 3.5 and higher from [Cran] (https://cran.r-project.org/)
* dplyr package
* psych package
* gridExtra package
* ggplot2 package
* knitr package


Install the necessary packages by running the following blocks of code in R

```{r}
installed_pkgs <- row.names(installed.packages())
pkgs <- c("dplyr", "psych", "gridExtra", "ggplot2", "knitr")
for(p in pkgs){
	if(!(p %in% install_pkgs)){
		install.packages(p)
	}
}
```
# Executing Analysis
The best way to execute this analysis is to run the following code

```{r}
Rscript -e "rmarkdown::render('costmodelling.Rmd')"
```
This would produce an HTML document showing results of the analysis

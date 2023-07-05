# Data Science Guides

A repository containing worked examples in R & Python of some common data science tasks, to use as a space for learning how to implement these methods, and as a template for applying data science to SCW work.

## Usage

### R/Python

In order to implement the guides in this repository, you will need to install R and/or Python (depending on which you wish to use). Getting R and Python installed on your local machine can prove to be a non-trivial task, and knowing which tools are best for using either language (especially Python) can sometimes act as a bit of a barrier for new users. To help reduce the barriers to entry for new users, there is a [notebook](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/getting-started.html) that takes you through some of these challenges, from getting either language installed on your local machine to which tools to use.

### Git

This repository relies on Git, a version control system, to manage the source code. This means that changes to the code (and anything else in the repository) can be tracked over time. This is a software engineering best-practice that has also been adopted in data science. It is an excellent 'habit' to learn when working with code, because it allows you to track changes, and therefore, revert to previous versions of the code if necessary. It also makes collaboration significantly easier, as it allows multiple people to work on the same codebase without creating conflicts.

If you are new to Git, a good place to start is the [NHS-R Git Training](https://github.com/nhs-r-community/git_training/). Their [Introduction to Git](https://github.com/nhs-r-community/git_training/blob/main/guides/introduction_to_git.md) will help you understand why version control is necessary, what Git & GitHub can offer, and how to navigate these tools.

These data science guides are designed to be used with Git because this is a very important skill for data science, and while it can be a bit challenging at first, it is incredibly valuable to learn, and everyone who wants to do some of the tasks in these guides should also be using Git to manage their work.

### Guides & Source Code

All guides are stored as html files in the /guides subdirectory, but they can be accessed from the links below. The source code for the guides are stored in the /src subdirectory. The source code (.qmd files) can be used to run the code locally.

The easiest way to use any of the guides is to clone this repository to your local machine so that you have all the files you need for setup.

### Setup

#### R

In order to run the R notebooks, you will first have to install all the packages that the code uses, and set up your R environment using [{renv}](https://rstudio.github.io/renv/articles/renv.html).

First, if you haven't already, install {renv}.

```{r}
install.packages("renv")
```

Having done this, you can now restore the R environment from the renv.lock file in the repository.

```{r}
renv::restore()
```

You should now be able to run all of the R notebooks in the repository. If you receive an error message, you may have to install certain packages manually. If you are unable to resolve any errors, please submit a [reproducible example](https://reprex.tidyverse.org/) as an [issue](https://github.com/NHS-South-Central-and-West/data-science-guides/issues) on the repository.

#### Python

In order to run the Python notebooks, you will first have to install all the packages that the code uses, and set up your Python environment using [pipenv](https://pipenv.pypa.io/en/latest/).

First, if you haven't already, install pipenv.

```{bash}
pip install pipenv
```

Having done this, you can now restore the Python environment from the Pipfile in the repository.

```{bash}
pipenv install
```

You should now be able to run all of the Python notebooks in the repository. If you receive an error message, you may have to install certain packages manually. If you are unable to resolve any errors, please submit a [reproducible example](https://stackoverflow.com/help/minimal-reproducible-example) as an [issue](https://github.com/NHS-South-Central-and-West/data-science-guides/issues) on the repository.

## Guides

### Getting Started

- [Identifying Data Science Opportunities](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/identifying_data_science_opportunities.html)
- A Scientific Approach to Answering Questions
- [Getting Started with R & Python](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/getting_started_with_r_and_python.html)
- [R vs Python](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/r_vs_python.html)
- Importing Data from SQL [[R](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/R/importing_data_from_sql.html)|[Python](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/python/importing_data_from_sql.html)]
- Data Wrangling [[R](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/R/importing_data_from_sql.html)|Python]
- Exploratory Data Analysis [[R](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/R/exploratory_data_analysis.html)|[Python](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/01-getting-started/python/exploratory_data_analysis.html)]

### Statistical Methods

- Hypothesis Testing (T-Test, ANOVA, Chi-Squared Test)
- Linear Regression [[R](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/02-statistical-methods/R/linear_regression.html)|[Python](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/02-statistical-methods/python/linear_regression.html)]
- Generalised Linear Models
- Generalised Additive Models
- Multilevel Regression
- Time Series Analysis & Forecasting

### Machine Learning

- Introduction to ML Concepts
- Designing Machine Learning Solutions
- End-to-End ML Workflow [[R](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/03-machine-learning/R/end_to_end_ml_workflow.html)|[Python](https://htmlpreview.github.io/?https://github.com/NHS-South-Central-and-West/data-science-guides/blob/main/guides/03-machine-learning/python/end_to_end_ml_workflow.html)]
  - Cross-Validation
  - Hyperparameter Tuning
- Unsupervised Learning (Clustering)
- Time Series Forecasting Using ML
- Gradient-Boosted Decision Trees

### Deep Learning

- Introduction to Deep Learning
- Image Classification
- Text Classification

### Delivering Data Science

- Introduction to Docker
- Introduction to Kubernetes
- Workflow Orchestration
- Reports & Presentations
- Web Apps & Dashboards
- APIs
- Data Pipelines

## Resources

- [R for Data Science](https://r4ds.hadley.nz/)
- [Telling Stories with Data](https://tellingstorieswithdata.com/)
- [StatQuest](https://www.youtube.com/@statquest)

## Acknowledgements

Several datasets used in this repository have been sourced from the following packages:

- [Fingertips](https://docs.ropensci.org/fingertipsR/)
- [NHS-R Datasets](https://nhs-r-community.github.io/NHSRdatasets/)
- [MLDataR](https://cran.r-project.org/web/packages/MLDataR/vignettes/MLDataR.html)

# blank_r_project
### A Project Skeleton for an R-Flavored Data Science Project

A template project directory for data science projects. Currently, this is set up for projects developed in R but should be easily adoptable to another language. Cloning this repo will give you the project directory detailed below. The analysis workflow is has pre-made R scripts which conform to the LFCD theory of analysis workflow. If you have data sources that require an API key or other private credential and store them in the connection secrets directory, **be sure to uncomment the line ignoring this directory in the project .gitgnore file** (there's a reminder in the directory name so hopefully you don't forget :stuck_out_tongue:).

Heavily adopted from:
* [cookie cutter data science project directory](https://github.com/drivendata/cookiecutter-data-science/blob/master/README.md)
* [LCFD Workflow](https://stackoverflow.com/questions/1429907/workflow-for-statistical-analysis-and-report-writing)

Directory Structure is as follows:
```
├── README.md          <- The top-level README for developers using this project.
├── analysis_workflow
│   ├── 00_functions.R       <- functions for use in analysis and data wrangling/munging
│   ├── 01_load.R        <- script to load data from various sources (csv, excel, db's, etc.) and save as .rda to prevent re-loading
│   ├── 02_clean.R      <- script to perform necessary cleaning/wrangling to get data in a usable form for analysis
│   ├── 03_analysis_model_train.R      <- script containing analysis and/or model training
│   ├── 04_model_prediction.R      <- script to apply model to new/test data
├── data
│   ├── cleaned       <- data ready to go for analysis
│   ├── connection_secrets_GIT_IGNORE        <- any API keys, passwords etc. Make sure to uncomment the gitignore line for this dir.
│   ├── data_sources      <- always document where things came from!
│   ├── interim      <- temp dir for data on it's way to being ready for analysis
│   └── raw            <- The original, immutable data dump.
│
├── documentation      <- project documentation
│
├── exploration_scratch <- scripts for general exploratory analysis 
│
├── markdown          <- directory for markdown documents
│
├── notes_lit         <- general analysis notes and papers/literature relevant to the project
│
├── output
│   ├── images       <- image files related to analysis
│   ├── models        <- trained models 
│   ├── tables      <- tabular outputs
│
├── shiny   <- directory for a shiny application if relevant
```

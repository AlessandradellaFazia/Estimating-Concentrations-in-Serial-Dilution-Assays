# Estimating-Concentrations-in-Serial-Dilution-Assays

This repository contains code written for the final project of the Bayesian Statistical Methods course, at Sapienza University of Rome.

The purpose of the project is estimating concentrations of compounds in biological samples using Bayesian hierarchical models within Markov Chain Monte Carlo (MCMC) simulation.

A common approach for estimating concentrations of compounds in biological samples is the *serial dilution assay*, in which a small amount of sample (or solute) are serially diluted, mixing a amount of sample with a measured amount of a inert liquid. Then for each diluted samples we take a measurement.The relation between concetrations and measurements is non linear and therefore it is not suitable to weight the measurements equally. Moreover, different dilutions give measurements with different accuracy.

The goal of the project is to estimates the concentration of a specific compound for a set of samples, using *standards* data (liquid solutions for which the concetration is known).

Given the small number of measurement available, a Bayesian approach is used. This approach makes it possible to exploit knowledge from biology inserted through the priority function. 

![Example of serial dilution](https://github.com/AlessandradellaFazia/Estimating-Concentrations-in-Serial-Dilution-Assays/blob/main/images/elisa.jpg)


Specifically, the repository collects the following files: 

- `SDSII Report Final Project della Fazia.Rmd`: R Markdown file containing the R code needed to reproduce the project, with text and graphic sections forming a data analysis document, readble with R Studio.
- `dilution.dat`: The dataset used.
- `R_Project.Rproj`: project file of R Studio.
- `.RData file`: load the data and values of the variables into R.
- `SDSII-Report-Final-Project-della-Fazia.html`: HTML version of the data analysis document, it can be read easily [here](https://htmlpreview.github.io/?https://github.com/AlessandradellaFazia/Estimating-Concentrations-in-Serial-Dilution-Assays/blob/main/SDSII-Report-Final-Project-della-Fazia.html).
- `SDSII-Report-Final-Project-della-Fazia.pdf`: PDF version of the same data analysis document.
- `simple_model_2.txt`: Text file defining the Bayesian graphical model (the simplest one), specified with in BUGS-language.
- `complex_model_2.txt`: Text file defining the second Bayesian model used. 

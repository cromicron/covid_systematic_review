# Systematic Review and Meta Analysis of Remdesivir for COVID-19 Treatment

This repository contains the code, data, and documentation for a systematic review and meta-analysis of the effectiveness of the drug Remdesivir in treating COVID-19. The goal of this project is to provide a clear and reproducible protocol for conducting a systematic review and meta-analysis, as well as to produce a meta-analysis of the findings of the included studies. This repository especially is intended to assist a researcher who wants to replicate the systematic review and meta-analysis.

## Background
Remdesivir is a drug that was first developed for the treatment of Ebola. It has been experimentally tested for use in Covid-19 patients, 
especially with those that suffered from pneumonia. It is a drug administered with an intravenous injection. <br>
A systematic review is a type of literature review which minimizes the individual researcher's bias on the results. It does so by
 following a well-specified pre-defined protocol on which studies to include for the analysis and which to exclude. 
The criteria are defined in advance of the literature search. Independent researchers should arrive at similar conclusions when they apply the given 
protocol. The purpose of this repository is to allow independent researchers to replicate the steps that the original author took in his analysis.
The population of studies this review is to be applied to, are publications found on PubMed-central - an open-access platform
 for biomedical publications. Among those, only studies which use a randomized-controlled-trial study-design are to be included in 
the analysis. Of those, only studies which report a ratio estimating the difference between Remdesivir and Control groups are to be 
included. The measures of interest are mortality-ratio and/or time to recovery or clinical improvement. Only majority adult studies
 with patients infected with Covid-19 are to be included in the analysis. <br>
Many steps in this analysis are automated. The tool Robotsearch is a machine-learning tool which tests PubMed-search results for randomized-
controlled trials. Further automation included the scanning of open access articles for proper outcome-measures. After the automated
steps are finished, the person replicating the review has to manually scan the remaining articles for eligibility. The Jupyter-notebook 
Conduct_Review.ipynb guides the person replicating through the steps necessary to evaluate the eligibility of studies based on the criteria mentioned
before. After having selected the proper studies, the replicator should extract the effect-measures, confidence-intervals, p-values,
sample-sizes from the studies and code if the study included a placebo-control group or a standard-care control-group. <br> 
The meta-analysis then can be automatically performed by running the code in the jupyter notebook. The final results are pooled effects
of ratios for mortality and time to recovery or clinical improvement with estimated confidence intervals, a forest-plot visualizing the
effects and two funnel-plots testing graphically for publication bias.


## Requirements and Dependencies

Installation of all requirements and dependencies is documented below under "running the code"


## Project Structure

The project is organized as follows:

- `Conduct_Review.ipynb`: A Jupyter Notebook to run the analyses.
- `env.yml`: A file to configure the virutal environment necessary with Anaconda.
- `README.md`: This file, containing an overview of the project and instructions for running the code.
- `robotsearch/`: Directory containing an adapted version of the external [repository](https://github.com/tarensanders/robotsearch) robotsearch to automate selection of randomized controlled trials.


## Running the Code

To run the code in this repository, follow these steps:
1. Clone or download the repository to your local machine. If you download, make sure to unzip the folder and extract to the directory of your choice.
2. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
3. Open the Anaconda Prompt and move into the project folder of this project by [using the cd command](https://www.lifewire.com/change-directories-in-command-prompt-5185508).
4. From anaconda run `conda env create -f env.yml` to create the environment with the required packages
5. Activate the environment by running `conda activate covid_review`
6. Install jupyter lab by running `pip install jupyter lab`
7. To use virtual environments within jupyter notebook run the following command `conda install -c anaconda ipykernel`
8. Install the kernel with the above created environment by running `python -m ipykernel install --user --name=covid_review` . Make sure to always activate the virtual environment before running jupyter.
9. Now install robotsearch. Move to the robotsearch-directory by typing `cd robotsearch`
10. Install robotsearch by executing `python setup.py install`
11. Go back to the project-root directory by executing `cd ../` and open the Jupyter Notebook by running `python -m jupyter lab Conduct_Review.ipynb`. 
12. Check the top right-hand corner for the kernel-name covid-review. If it shows another kernel - e.g. python3, click on the name and choose covid_review.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

We would like to thank the authors of the included studies for their contributions to our systematic review and meta analysis. We would also like to thank [IJ Marshall](https://github.com/ijmarshall/robotsearch) and [Taren Sanders](https://github.com/tarensanders/robotsearch) for the open-source tool robotsearch. We would also like to thank Openai for their open source tool [Chat-GPT](https://chat.openai.com/chat) which assisted this project and generated the code-structure for this file.


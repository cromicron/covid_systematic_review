# Systematic Review and Meta Analysis of Remdesivir for COVID-19 Treatment

This repository contains the code, data, and documentation for a systematic review and meta analysis of the effectiveness of the drug Remdesivir in treating COVID-19. The goal of this project is to provide a clear and reproducible protocol for conducting a systematic review and meta analysis, as well as to produce a meta analysis of the findings of the included studies. This repository especially is intended to assist a reasearcher who wants to replicate the systematic review and meta-analysis.


## Requirements and Dependencies

Installation of all requirements and dependencies is documented below under "running the code"


## Project Structure

The project is organized as follows:

- `Conduct_Review.ipynb`: A Jupyter Notebook to run the analyses.
- `env.yml`: A file to configure the virutal environment necessary with Anaconda.
- `README.md`: This file, containing an overview of the project and instructions for running the code.
- `robotsearch/`: Directory containing an adabted version of the external [repository](https://github.com/tarensanders/robotsearch) robotsearch to autmate selection of randomized controlled trials.


## Running the Code

To run the code in this repository, follow these steps:
1. Clone or download the repository to your local machine.
2. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
3. Open the Anaconda Prompt and move into the project folder of this project by [using the cd command](https://www.lifewire.com/change-directories-in-command-prompt-5185508).
4. From anaconda run `conda env create -f env.yml` to create the environment with the required packages
5. Activate the environment by running `conda activate covid_review`
6. Install jupyter lab by running `pip install jupyter lab`
7. To use virtual environments within jupyter notebook run the following command `conda install -c anaconda ipykernel`
8. Install the kernel with the above created environment by running `python -m ipykernel install --user --name=covid_review` . Make sure to always activate the virtual envoironment before running jupyter.
9. Now install robotsearch. Move to the robotsearch-directory by typing `cd robotsearch`
10. Install robotsearch by executing `python setup.py install`
11. Go back to the project-root directory by executing `cd ../` and open the Jupyter Notebook by running `python -m jupyter lab Conduct_Review.ipynb`. 
12. Check the top right-hand corner for the kerne-nam covid-review. If it shows another kernel - e.g. python3, click on the name and choose covid_review.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

We would like to thank the authors of the included studies for their contributions to our systematic review and meta analysis. We would also like to thank [IJ Marshall](https://github.com/ijmarshall/robotsearch) and [Taren Sanders](https://github.com/tarensanders/robotsearch) for the open-source tool robotsearch. We would also like to thank openai for their open source tool [chatgpt](https://chat.openai.com/chat) which assisted this project and generated the code-structure for this file.


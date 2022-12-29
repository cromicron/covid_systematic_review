# Systematic Review and Meta Analysis of Remdesivir for COVID-19 Treatment

This repository contains the code, data, and documentation for a systematic review and meta analysis of the effectiveness of the drug Remdesivir in treating COVID-19. The goal of this project is to provide a clear and reproducible protocol for conducting a systematic review and meta analysis, as well as to produce a meta analysis of the findings of the included studies. This repository especially is intended to assist a reasearcher who wants to replicate the systematic review and meta-analysis.

## Project Components



## Requirements and Dependencies

Installation of all requirements and dependencies is documented below under "running the code"


## Project Structure

The project is organized as follows:

- `Conduct_Review.ipynb`: A Jupyter Notebook to run the analyses.
- `Protocol.md`: The Protocol to conduct the systematic review.
- `README.md`: This file, containing an overview of the project and instructions for running the code.
- `robotsearch/`: Directory containing an adabted version of the external [repository](https://github.com/tarensanders/robotsearch) robotsearch to autmate selection of randomized controlled trials.


## Running the Code

To run the code in this repository, follow these steps:
1. Clone or download the repository to your local machine.
2. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
3. Open the Anaconda Prompt and cd into the project folder of this project
4. From anaconda run `conda env create -f env.yml` to create the environment with the required packages
5. To use virtual environments within jupyter notebooks run the following command `conda install -c anaconda ipykernel`
6. Install the kernel with the above created environment by running `python -m ipykernel install --user --name=covid_review`
7. Open the Jupyter Notebook `Conduct_Review.ipynb`. Choose the kernel covid_review created above and follow the instructions carefully.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

We would like to thank the authors of the included studies for their contributions to our systematic review and meta analysis. We would also like to thank [R](https://www.r-project.org/), [metafor](https://cran.r-project.org/package=metafor), and [rmarkdown](https://rmarkdown.rstudio.com/) for their powerful tools for conducting systematic reviews and meta analyses. We would also like to thank openai for their open source tool [chatgpt](https://chat.openai.com/chat) which assisted this project and generated the code-structure for this file.


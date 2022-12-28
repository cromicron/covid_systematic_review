# Systematic Review and Meta Analysis of Remdesivir for COVID-19 Treatment

This repository contains the code, data, and documentation for a systematic review and meta analysis of the effectiveness of the drug Remdesivir in treating COVID-19. The goal of this project is to provide a clear and reproducible protocol for conducting a systematic review and meta analysis, as well as to produce a meta analysis of the findings of the included studies.

## Project Components

This project consists of three main components:

1. Protocol development: A detailed protocol for conducting a systematic review and meta analysis is provided, including the selection criteria for included studies and the methods for data extraction and analysis.

2. Systematic review: The protocol is followed to conduct a systematic review of the effectiveness of Remdesivir in treating COVID-19. The review includes a description of the search strategy, the inclusion and exclusion criteria, and the characteristics of the included studies.

3. Meta analysis: A meta analysis of the findings of the included studies is conducted using appropriate statistical methods. The results of the meta analysis are presented in a clear and concise manner, including a summary of the main findings and any limitations of the analysis.

## Requirements and Dependencies

This project requires the following software and libraries:

- [R](https://www.r-project.org/) (version 3.6 or higher)
- [RStudio](https://rstudio.com/) (optional, but recommended)
- [metafor](https://cran.r-project.org/package=metafor) package for R
- [rmarkdown](https://rmarkdown.rstudio.com/) package for R

## Project Structure

The project is organized as follows:

- `data/`: Directory containing the data files for the systematic review and meta analysis.
- `notebooks/`: Directory containing the Jupyter notebooks for the protocol development, systematic review, and meta analysis.
- `output/`: Directory containing the output files (e.g. PDFs, HTML files) generated from the Jupyter notebooks.
- `README.md`: This file, containing an overview of the project and instructions for running the code.

## Running the Code

To run the code in this repository, follow these steps:
1. Clone or download the repository to your local machine.
2. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
3. Open the Anaconda Prompt and cd into the project folder of this project
4. From anaconda run `conda env create -f env.yml` to create the environment with the required packages
5. To use virtual environments within jupyter notebooks run the following command `conda install -c anaconda ipykernel`
6. Install the kernel with the above created environment by running `python -m ipykernel install --user --name=covid_review`
7. Open the Jupyter notebooks in the `notebooks/` directory and run the code cells to reproduce the results of the protocol

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

We would like to thank the authors of the included studies for their contributions to our systematic review and meta analysis. We would also like to thank [R](https://www.r-project.org/), [metafor](https://cran.r-project.org/package=metafor), and [rmarkdown](https://rmarkdown.rstudio.com/) for their powerful tools for conducting systematic reviews and meta analyses. We would also like to thank openai for their open source tool [chatgpt](https://chat.openai.com/chat) which assisted this project and generated the code-structure for this file.


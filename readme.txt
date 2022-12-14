This repository contains a dataset on malicious bidding and associated analysis code. This dataset is licensed under a CC BY 4.0 license (https://creativecommons.org/licenses/by/4.0/).

The dataset is contained in the 'dataset' directory, and consists of 2 txt files and 4 csv files:
- subject_areas.txt contains the 25 subject areas used.
- papers.txt contains the titles of the 28 papers used.
- setup.csv contains the reviewer profiles constructed during activity setup.
- honest_bidding.csv contains the responses to the honest bidding phase of the activity.
- malicious_bidding.csv contains the responses to the malicious bidding phase of the activity.
- strategy_annotations.csv contains our strategy labels for the malicious reviewers.

The file parse_data.py reads the dataset files and saves them in an appropriate format for the analysis script. Before running this file, construct a directory for the output with:
	'mkdir analysis/data'

The 'analysis' directory contains analysis scripts:
- analysis.py contains the code for analysis of the original dataset.
- synthetic.py contains code for analysis of the scaled-up dataset.
- plot.ipynb contains code to generate plots.
These scripts should be run from the 'analysis' directory.

# ML-Final-Project

(c) Emma Neil 2022

This repository contains a Juypter notebook with code for predicting non-residential building energy usage using an ANN and logistic regression on the Building Data Genome Project 2 dataset. 

According to the U.S. Energy Information Administration, non-residential energy consumption accounts for 12% of total energy usage nationally (USE, 2021). As we, as a nation, tackle reducing the energy consumption of this sector, it is important to be able to identify the most inefficient buildings in our national housing stock and what contributes to their high energy usage. Without precise and consistent readings from a variety of energy me- ters, it can be difficult for building managers, architects, or municipalities to acquire the necessary information to flag such buildings and prioritize them for either renovation or destruction.

For this project, I train an Artificial Neural Network (ANN) with a baseline Logistic Regression to predict, categorically, whether a non-residential building will consume energy efficiently in 2017 based on non-metered information about the building and limited meter data documenting its energy consumption in 2016. I lean on the US Department of Energy’s Source Energy Use Intensity (EUI) statistic to determine whether a building’s energy consumption counts as efficient. Both models achieved higher accuracy than a naive classifier-- the ANN was 96.3% accurate on the test data while the baseline was 94.8% accurate.

### Run the Notebook ###

1. Clone the repository using `git clone` followed by the SSH or HTTPS URL.

2. Download the following CSVs from the [Kaggle Building Data Genome Project 2](https://www.kaggle.com/datasets/claytonmiller/buildingdatagenomeproject2?select=solar_cleaned.csv) dataset:

* electricity_cleaned.csv
* solar_cleaned.csv
* gas_cleaned.csv
* metadata.csv
  
3. Create a directory within this repository on your local machine titled "building_genome_datasets/" with the command `mkdir building_genome_datasets/` and move the CSVs into this directory.

4. Install Jupyter Notbook with the command `pip install notebook` or `pip3 install notebook`. Then run the notebook from inside the repository with the command `jupyter notebook`.

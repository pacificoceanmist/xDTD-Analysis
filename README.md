# xDTD Analysis

## Overview

The xDTD Analysis repository is dedicated to the investigation and analysis of variances in KGML-xDTD models, with a focus on random forest (RF) prediction probabilty performance. This project is a part of the 6 week rotation project at David Koslicki Lab.

## Rotation Project Objectives

1. **Investigate Schema Variances Between the Models:**
   - Explore and analyze differences between xDTD models.
   - Examine each model's schema characteristics and trends.
   
2. **Investigate RF Prediction Probability Performance:**
   - Examine RF prediction probability results for 100 drug-disease pairs.
   - Assess prediction performance variance for each model.

## Repository Contents
Each scripts contain data location and instructions necessary to perform each analysis. To conduct the analysis use the scripts in the following order below:

1. `xDTD_Schema_Analysis_Scripts` contains scripts for schema analsysis for `Node Mapping`, `Path Result`, and `Drug-Disease Pairs`.

2. `xDTD_Drug-DiseasePairs_Extract` contains script to extract drug-disease pairs. The directory also contains 154 drug-disease pairs used for the rotation project in CSV file format.

3. `xDTD_RandomForest_Instruction` contains script to run the random forest mode to obtain the drug-disease prediction probabiltiy.

4. `xDTD_RandomForest_Prediction_Analysis` is the final step in analysis. It contains script to extract prediction probability scores of hundred drug-disease pairs and visualization, scatter plot, of the result.

## Jupyter Notebook Script

The core of the analysis is encapsulated in the Jupyter notebook script. This script contains the necessary code and instructions to perform the KGML-xDTD analysis, addressing the rotation project objectives.

### Figures

The folder holds the visual output results of the analysis. These results are presented in both PDF, PNG, and JPEG formats.

### Pre-Setting
1. Install [Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html).
2. Obtain `.yml` files for the conda environment from [here](https://github.com/RTXteam/xDTD_training_pipeline/blob/master/envs/xDTD_training_pipeline_env.yml).
2. Install conda environments using the following commands:
```
# Install Mamba
conda install -c conda-forge mamba

# Configure conda environments
mamba env create -f envs/graphsage_p2.7env.yml
mamba env create -f envs/xDTD_training_pipeline_env.yml

# Activiate the 'xDTD_training_pipeline' conda environment
conda activate xDTD_training_pipeline
```
### Start of Analysis
To begin your analysis or reproduce the results, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/xDTD-Analysis.git

2. Navigate the project directory:

   ```bash 
   cd xDTD-Analysis
   ```

4. Import, or download, and decompress the data files. The location of the data for each analysis is provided in each Jupyter Notebook script.

4. Open and run the Jupyter notebook scripts:
   ```bash
   jupyter notebook <name_of_the_script>.ipynb
   ```
This will initiate the analysis and generate the results.

## Note: ##

We recommend you have the following specifications to successfuly run the pipeline and the scripts.

• Operating system(s): Linux (Ubuntu)

• Programming language: Shell Script (Bash) and Jupyter Notebook Script with Python 3.8.12

• Other requirements: Mamba version 1.5.0 and Anaconda version 23.7.4

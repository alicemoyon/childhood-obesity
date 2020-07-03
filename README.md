## Analysis of the nature and causes of childhood obesity in England for the Guy's and St Thomas' charity

### Background

Guy's and St Thomas' Charity is an independent, place-based foundation working to improve the health of people in the London boroughs of Lambeth and Southwark.
To achieve this, they are concentrating on a small number of programmes focused on key health issues.

In this project they are focusing on the issue of childhood obesity in Lambeth and Southwark.

### Objectives

The aim of this project is for Guy’s & St Thomas’ Charity to understand where to target its resources and which areas to fund in the London boroughs of Lambeth and Southwark, to help childhood obesity levels and its effects. This will involve:

* Identifying places most (and least) affected by childhood obesity
* Identifying who lives in the areas, using a range of socio demographic data
* Identifying what the contributing factors are. e.g. by exploring pollutant concentration levels, emissions data and sources of emissions with a particular focus on traffic and time
* Identifying how the childhood obesity has evolved over time
* Identifying neighborhoods across the UK that have similar characteristics to neighborhoods in Lambeth and Southwark with high obesity rates.

Ultimately, my more advanced goal with this project is to explain the nature and causes of childhood obesity in England (with a focus on Lambeth and Southwark) in order to provide actionable insights on what specific root causes to target.

### Data

All the data is in CSV and split into 3 files:

ReceptionObese.csv - contains Reception (4/5 year olds) obesity rates over time</br>
Year6Obese.csv - contains Year 6 (10/11 year olds) obesity rates over time</br>
SocioDemographicData.csv - contains a lot of data on the sociodemographic side (~170,000 rows by 118 Columns)

All the data is a row per MSOA or LSOA - These are UK statistical areas used and defined during the census, they are approx. 1000 people. It should be noted that some data has been aggregated down. This is from MSOA, which is the next level of the Hierarchy. LSOAs fit perfectly into MSOA, which fit into LA. For example, Southwark 003A (LSOA) is within Southwark 003 (MSOA) that is within Southwark (LA). All the data is within England.

A corresponding data dictionary is also included (FullDataDictionary.csv)

### Approach

Initially, I will conduct exploratory data analysis by applying statistical methods using Python and generating some data visualisations.

Phase 1: Explore the obesity data</br>
Phase 2: Explore the sociodemographic data</br>
Phase 3: Find correlations and derive causal insights from the two sets of data

NB: **This is a work in progress**. As I learn more advanced techniques, I will apply them to the data to gain further insights as well as produce interactive data visualisations. This will hopefully include using PCA to reduce the dimensionality of the data, applying Causal Inference methods and machine learning if appropriate.
The Jupyter Notebook shows all the details of the data exploration and all the intermediate steps and visualisations. It is not the final product that would be presented to the charity. A final presentation containing only the relevant insights and visualisations will be put together once the project is completed.

### Running the notebook

The full data analysis is contained in the **gsttcharity.ipynb** notebook. In order to execute the code in the notebooks, you need to create an Anaconda environment and install the python packages listed in the requirements file included in this repository.

If you do not have Anaconda already installed, you can download it here https://www.anaconda.com/products/individual

Once Ananconda is installed on your machine, you can then create a new conda environment with the required packages by running the following on the command line:
conda create --name yourenvname --file conda_childhoodobpy38_requirements.txt

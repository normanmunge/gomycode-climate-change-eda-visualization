Data Wrangling/Munging and Visualization to analyze Climate Change in Africa

Africa is the most vulnerable continent to climate change impacts under all climate scenarios above 1.5 degrees Celsius. Despite having contributed the least to global warming and having the lowest emissions, Africa faces exponential collateral damage, posing systemic risks to its economies, infrastructure investments, water and food systems, public health, agriculture, and livelihoods, threatening to undo its modest development gains and slip into higher levels of extreme poverty. (African Development Bank Group)[https://www.afdb.org/en/cop25/climate-change-africa]

For data scientists or anyone interested in climate, there are signs that you can check to identify changes in climate. Some of these include:

- Rising Temperatures
- Longer and extreme droughts in the world
- Increase in severe tropical storms
- Increase in sea levels

This project explores the daily temperatures and precipitation recorded in five countries (Angola, Tunisia, Cameroon, Senegal, Egypt) from 1980 to 2023. The dataset was provided by the (US Global Change Research Program)[https://www.globalchange.gov/] and you can access it using this link [https://drive.google.com/file/d/1I8eV4-8p61CNNlVJzzho2xeoZ5-P7Q0F/view].

## 1. <a name='TableofContents'></a>Table of Contents

<!-- vscode-markdown-toc -->

- 1. [Table of Contents](#TableofContents)
- 2. [Objectives, Planning and Folder Structure](#ObjectivesPlanningandFolderStructure)
  - 2.1. [Objectives](#Objectives)
  - 2.2. [Folder Structure](#FolderStructure)
- 3. [Setting up in your local environment](#Settingupinyourlocalenvironment)
  - 3.1. [Creating a virtual environment](#Creatingavirtualenvironment)
  - 3.2. [Activating your environment](#Activatingyourenvironment)
  - 3.3. [Deactivating your environment](#Deactivatingyourenvironment)
- 4. [Libraries and Installations](#LibrariesandInstallations)
  - 4.1. [Required Libraries](#RequiredLibraries)
  - 4.2. [Installation](#Installation)
- 5. [Starting your notebook](#Startingyournotebook)
- 6. [Disclaimer - use analysis with caution](#Disclaimer-useanalysiswithcaution)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

## 2. <a name='ObjectivesPlanningandFolderStructure'></a>Objectives, Planning and Folder Structure

### 2.1. <a name='Objectives'></a>Objectives

The [notebook](/climate_change_africa.ipynb) does an exploratory data analysis on the data using a pandas DataFrame. The objectives of the project is to:

1. Load the dataset from csv's
2. Cleaning of the data - missing values, wrong values, duplicate values
3. A statistical summary on the numerical features
4. Analysis of the following questions:
   - Annual Average temperature per country
   - How temperature affects precipitation
5. Visualization of the answered questions above

### 2.2. <a name='FolderStructure'></a>Folder Structure

The repository contains:

Datasets Directory - This directory holds our dataset - [Africa_climate_change.csv](/datasets/Africa_climate_change.csv, 'African climate change dataset') The notebook contains the columns below:

- date
- prcp - Daily Precipitation
- tavg - Daily Average Temperature
- tmax - Daily Maximum Temperature
- tmin - Daily Minimum Temperature
- country

2. [Requirements.txt] (/requirements.txt) - Showing the necessary libraries and dependencies to run the notebook.
3. Notebooks
   - [climate_change_africa notebook](climate_change_africa.ipynb)
4. [Gitignore File](/.gitignore) - File to ignore files and directories from being pushed to the remote repository
5. [README.md File](/README.md) - Guiding instructions for describing and running the project.

## 3. <a name='Settingupinyourlocalenvironment'></a>Setting up in your local environment

This section guides you on how to setup your environment and run the repository on your local environment.

### 3.1. <a name='Creatingavirtualenvironment'></a>Creating a virtual environment

Create a virtual environment to install and manage the libraries to isolate them from your global environments.

To create a virtual environment, run the command below on your terminal:

```bash
python -m venv 'myenv_name'
```

### 3.2. <a name='Activatingyourenvironment'></a>Activating your environment

To activate your environment on linux or mac operating system. Run the command below on your terminal.

```bash
source /path/to/myenv_name/bin/activate
```

To activate your environment on a windows environment:

```bash
source \path\to\myenv_name\Scripts\activate
```

### 3.3. <a name='Deactivatingyourenvironment'></a>Deactivating your environment

Once you're done working on the repository, REMEMBER to deactivate your virtual environment in order to separate your local project dependencies.

To deactivate your environment on a linux or mac operating system. Run the command below on your terminal:

```bash
deactivate
```

## 4. <a name='LibrariesandInstallations'></a>Libraries and Installations

### 4.1. <a name='RequiredLibraries'></a>Required Libraries

The important libraries used in this environment are:

1. Pandas - Used for manipulation, exploration, cleaning and analyzing of your dataset.
2. Plotly - Used for visualization purposes to highlight discovered patterns in your dataset to stakeholders in form of graphs
3. Jupyter lab - Used to run and experiment on your notebook in your local environment

The above listed libraries are the core ones used in the repository. However, during installation you'll notice other dependencies installed that enable to work as expected. They are highlighted on the [requirement.txt](/requirements.txt) file.

### 4.2. <a name='Installation'></a>Installation

Ensure you are have a version python > 3 installed and running on your local environment in order to to be able to install the libraries and run the notebook. Afterwards, ensure the virtual environment you created above is active before running the installation commands below on your terminal.

To install the libraries run:

```bash
pip install pandas plotly jupterlab
```

You can also install all the libraries by running:

```bash
pip install requirements.txt
```

## 5. <a name='Startingyournotebook'></a>Starting your notebook

To run your notebook in your local environment, we'll require the jupyter lab library installed. Afterwards, run the command below on your terminal:

```bash
jupyter lab *optional_file_name*
```

## 6. <a name='Disclaimer-useanalysiswithcaution'></a>Disclaimer - use analysis with caution ⚠️

1. The dataset is purely for learning purposes and hasn't been verified hence it isn't advisable to use it in a business setting as it might contain a wrong depiction of the climate changes in the listed countries.

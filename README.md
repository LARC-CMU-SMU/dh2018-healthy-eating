
# Does Journaling Encourage Healthier Choices? Analyzing Healthy Eating Behaviors of Food Journalers

This repository contains the dataset and two Jupyter notebooks used for reproducing the results published in our [Digital Health 2018 paper](https://www.researchgate.net/publication/323956631_Does_Journaling_Encourage_Healthier_Choices_Analyzing_Healthy_Eating_Behaviors_of_Food_Journalerse).

Please contact [Aek](mailto:palakorna@smu.edu.sg?cc=palakorn@gmail.com) if you have any questions or problems.

## Requirements
The notebooks have been tested in Python 2.7 with the following packages:

* Pandas 0.23
* Matplotlib 2.2.3
* Seaborn 0.9
* Scikit-learn 0.20.2

See requirements.txt for a complete list.

## Project Structure
By default, the project assumes the following directory structure:
```
project 
└───data  
│   │   profiles.csv
│   │   fv_servs.csv
│   │   protein_servs.csv
│   │   sugar_servs.csv
│   │   diary_days.csv
│   │   lapses.csv
└───notebooks
│   │   1-exploratory-data-analysis.ipynb
│   │   2-stats-regression-analysis.ipynb
│   │   [optional]-streaks-lapses.ipynb
└───reports
│   └───figures
```
All CSV data files should be put in the `data` folder. All notebooks should be put in the `notebooks` folder. Any generated reports and figures will be put in the `reports` folder.

## Pipeline

### Step 0: Data import
[Download the data](https://drive.google.com/open?id=1z8iJZHJMnEAHSSCsKbdyUR7N9ccVuveH) and extract the CSV files to the `data` directory.

### Step 1: Exploratory data analysis
Run the notebook `1-exploratory-data-analysis.ipynb` to generate figures and additional aggregated food intake data.

__Outputs:__ Several CSV files will be generated and stored in the `data` folder.

### Step 2: Hypothesis testing and regression analysis
Run the notebook `2-stats-regression-analysis.ipynb` to perform hypothesis testing and regression analysis of food intakes. The notebook requires data files from previous steps in the `data` folder.

__Outputs:__ Several reports will be generated and stored in the `reports` folder.

### [Optional] Analyzing streaks and lapses

Run the notebook `[optional]-streaks-lapses.ipynb` to compute logging streaks and lapses.

__Outputs:__ Several CSV files will be generated and stored in the `data` folder.

# ClothingFitnessPrediction
This repo contains our work on ModCloth &amp; RentTheRunWay datasets for processing and fitness prediction.

## **DataProcessingVisualizationPipeline.ipynb**
This file contains pipeline code for following things:
- Mounting of Google drive
- Loading datasets from json files to dataframe
- Imputing missing values for each feature
- Visualizing relationship of each feature with dependent variable *"fit"* for each item category in dataset

The already executed file showing cell outputs can be accessed from [here](https://drive.google.com/file/d/1K7DS7rU7QyezsJMwdvL5NTXWAxMjAcPY/view?usp=sharing). 

## **MLPipeline.ipynb**
This file contains pipeline code for following things:
- Data Processing without any visualizations
- Final assembling of dataframe
- Converting categorical to numerical variables
- Implementing GridSearchCV for hypertuning
- ML models & their classification report for both datasets

The already executed file showing cell outputs can be accessed from [here](https://colab.research.google.com/drive/1tDbGgiZRe-WfS4ZzdjqsowWiGYSNp1bD?usp=sharing).

## **Datasets.zip**
This is a zipped file that contains a folder titled *"Datasets"*. This folder contains two json files namely:
- modcloth.json
- renttherunway.json

The reference for where we got the datasets for the project is as follows: 
> Rishabh Misra, Mengting Wan, and Julian McAuley. 2018. Decomposing fit semantics for product size recommendation in metric spaces. In Proceedings of the 12th ACM Conference on Recommender Systems (RecSys '18). Association for Computing Machinery, New York, NY, USA, 422–426. DOI:https://doi.org/10.1145/3240323.3240398.

## **Steps to run .ipynb files**
The uploaded .ipynb files are configured to mount Google drive and read datasets from a folder present in *"My Drive"*. It can easily be configured to be run locally, by removing Google drive mount section. Also, update the path of the files location in **read_json()** function, which reads data from json files into a dataframe.

# halting-problem-sql
It is possible to predict exectution time of a SQL query with ML?

I'have named this repository after it's main objective remind me a well known problem known as halting problem, by Alan Turing, wich states, poorly speaking, that you cannot know if a program will terminate before you execute it. However will be intriguing use statistical model to find out what happen.

---

### Contents and Instruction:  
  
This repository contains files related to to `SQL Analytics Problem` [available here](https://github.com/claranet-coast/sql-analytics-problem) and provide a possible solution for takling the problem:

1. `Data_Analytics.ipynb` It's a Jupyter Notebook file focused on analyzie the raw data with some transformations, feature extraction and graphic visualization. Executing this file will produce a *Dataset* csv file suitable for next step: model training.
2. `Model_Training.ipynb` It's a Jupyter Notebook file focused on preprocess the *Dataset* created after the analytics phase described before. It define a preprocessor, pipeline, and test some models performance ending up with a selected model ready for use.
3. `queries_dataset.csv` It's the .csv file that will be created executing `Data_Analytics.ipynb`.
4. `query_time_predictor.model` It's a file that will be created executing `Model_Training.ipynb` and contains the choosen model serialization.
5. `requirements.txt` Has been created with command `pip freeze > requirements.txt` and contains all the available packages and version in the development environment.
6. `data` folder contains the original raw data from the linked repository.

---

* If all dependecies are satisfied, run `Data_Analytics.ipynb` and then `Model_Training.ipynb`.
* Optionally, if all dependencies are satisfied, and you are interested only in model training, run `Model_Training.ipynb`, a pre-generated *Dataset* is provided.
